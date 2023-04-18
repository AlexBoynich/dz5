<template>
  <div id="app" class="container">
    <Header msg="Navigation Menu"
    v-bind:navMenu="navMenu"
    />
    <About
    v-for="info of information" 
    v-bind:info="info"
    />
    <Skills
    v-bind:summary="summary"
    />
    <SocialNetworks class="social-networks-block" id="social"/>
    <LastPosts
    v-bind:lastPosts="lastPosts"
    />
    <ContactUs
    />
  
    <Footer 
    v-for="foot of footy"
    v-bind:foot="foot"
    />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Skills from './components/Skills.vue';
import About from './components/About.vue';
import Footer from './components/Footer.vue';
import ContactUs from './components/ContactUs.vue';
import SocialNetworks from './components/SocialNetworks.vue';
import LastPosts from './components/LastPosts.vue';

export default {
  name: 'App',
  data() {
    return {
      navMenu: [
        {title: 'ABOUT'},
        {title: 'SKILLS'},
        {title:'SOCIAL'},
        {title:'CONTACT US'},
        {title:'BLOG'}
      ],
      summary: [
        {title: 'Html', p:"Do you sometimes have the feeling that you're running into the same obstacles over and over again? Many of my conflicts have the same feel to them, like “Hey, I think I’ve been here before,” but I can’t figure out how I wound up in the same place.<br> <br>The situation is different, but the conflict feels the same. I first read this poem in “The Tibetan Book of Living and Dying” by Sogyal Rinpoche. When I “Googled” it, I found fourteen pages of links. It’s clearly a favorite with many people; I know it speaks volumes to me. “Autobiography in Five Chapters”"},
        {title: 'CSS', p:"Do you sometimes have the feeling that you're running into the same obstacles over and over again? Many of my conflicts have the same feel to them, like “Hey, I think I’ve been here before,” but I can’t figure out how I wound up in the same place.<br> <br>The situation is different, but the conflict feels the same. I first read this poem in “The Tibetan Book of Living and Dying” by Sogyal Rinpoche. When I “Googled” it, I found fourteen pages of links. It’s clearly a favorite with many people; I know it speaks volumes to me. “Autobiography in Five Chapters”"},
        {title: 'JavaScript', p:"Do you sometimes have the feeling that you're running into the same obstacles over and over again? Many of my conflicts have the same feel to them, like “Hey, I think I’ve been here before,” but I can’t figure out how I wound up in the same place.<br> <br>The situation is different, but the conflict feels the same. I first read this poem in “The Tibetan Book of Living and Dying” by Sogyal Rinpoche. When I “Googled” it, I found fourteen pages of links. It’s clearly a favorite with many people; I know it speaks volumes to me. “Autobiography in Five Chapters”"},
        {title: 'Vue', p:"Do you sometimes have the feeling that you're running into the same obstacles over and over again? Many of my conflicts have the same feel to them, like “Hey, I think I’ve been here before,” but I can’t figure out how I wound up in the same place.<br> <br>The situation is different, but the conflict feels the same. I first read this poem in “The Tibetan Book of Living and Dying” by Sogyal Rinpoche. When I “Googled” it, I found fourteen pages of links. It’s clearly a favorite with many people; I know it speaks volumes to me. “Autobiography in Five Chapters”"}
      ],
      information: [
        {name: 'Alex', spec: 'frontend-developer', scroll: 'Scroll to more'}
      ],
      footy: [
        {text:'Copyright © 2023. All rights reserved.'}
      ],
      lastPosts: [
                {title:'There are many reasons to get down', text: 'The only moment, the only life we have is in the NOW. What happened a few moments or several years ago is gone, what will happen this evening, or next month when we go on holidays is not here yet.', date: '10	Oct 21'},
                {title:'Choosing The Right Path', text: 'Although this is well intentioned and the goal certainly is to reduce the quantity of these bothersome thoughts, the technique is inherently flawed. Requiring the individual to remember what not to think of infers that they have already thought it. It is akin to telling them to not think of a blue banana.', date: '58	Oct 20'},
                {title:'Start your journey here', text: 'The only moment, the only life we have is in the NOW. What happened a few moments or several years ago is gone, what will happen this evening, or next month when we go on holidays is not here yet.', date: '29	Oct 18'}
            ]
    }
  },
  components: {
    Header,
    Skills,
    About,
    Footer,
    ContactUs,
    SocialNetworks,
    LastPosts

  }
}
</script>

<style>
@import "../src/stylesApp.css"
</style>
