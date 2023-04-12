<template>
    <div class="container">
        <p>{{ foot.text }}</p>
    </div>
</template>

<script>
export default {
    props: {
        foot: {
            type: Object,
            required: true
        }
    }
}
</script>

<style scoped>
p{
    display: flex;
    justify-content: center;
}
</style>