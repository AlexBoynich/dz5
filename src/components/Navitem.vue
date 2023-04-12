<template>
    <li>
       <a href="#">{{nav.title}}</a>
    </li>
</template>

<script>
export default {
    props: {
        nav: {
            type: Object,
            required: true
        }
    }
}
</script>

<style scoped>
    li{
        display: block;
        padding: 0 20px;
    }
    a{
        text-decoration: none;
    }
    a:hover {
        color: #6E38F7;
    }
</style>