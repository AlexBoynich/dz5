<template>
    <div class="header container">
        <img alt="Vue logo" src="../assets/logo.png">
        <img class="burger" src="../assets/Burger.png" alt="">
        <ul>
            <Navitem
            v-for="nav of navMenu"
            v-bind:nav="nav"
            />
        </ul>
    </div>
</template> 

<script>
import Navitem from './Navitem.vue';
    export default {
        props: ['navMenu'],
        components: {
            Navitem
        }

}
</script>

<style scoped>
.header{
    display: flex;
    justify-content: space-between;
}
ul{
    list-style-type:none;
    display: flex;
    flex-direction: row;
    margin: 0;
}
img {
  display: flex;
  width: 36px;
  height: 36px;
}
.burger{
    display: none;
}

@media (max-width: 920px) {
    .header{
        padding: 0;
        position: relative;
        z-index: 2;
    }
    ul{
        display: none;
    }
    .burger{
        display: block;
    width: 17px;
    height: 12px;
}
}
</style>