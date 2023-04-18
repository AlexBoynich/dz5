<template>
    <section>
        <h2>My social networks</h2>
        <p class="small-paragraph">There are many reasons to get down and start to get depressed about your situation.</p>
        <Slider/>
    </section>
</template>

<script>
    import Slider from '@/components/Slider.vue';
    export default {
        name: 'SocialNetworks',
        components: {
            Slider
        }
    }
</script>

<style scoped>
section {
    display: flex;
    flex-direction: column;
}
    h1 {
        margin-bottom: 20px;
    }
    p {
        margin-bottom: 40px;
    }
    .small-paragraph{
        max-width: 100%;
    }
</style>