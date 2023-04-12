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
    <Slider/>
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
import Slider from './components/Slider.vue';

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
      buttonProps: [
        {text: 'SEND'}
      ],
      Inputs: [
        {type: 'text'},
        {type: 'text'}
      ]
    }
  },
  components: {
    Header,
    Skills,
    About,
    Footer,
    ContactUs,
    Slider

  }
}
</script>

<style>
@import "../src/stylesApp.css"
</style>
