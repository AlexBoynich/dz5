<template>
    <div class="post">
        <img src="../assets/postImage.png" alt="">
        <div class='content'>
            <h4>{{ post.title }}</h4>
            <p class="postText">{{ post.text }}</p>
            <div class="dateAndA">
                <p class="small-paragraph">{{ post.date }}</p>
                <a href="#">READ MORE</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        post: {
            type: Object,
        }
    }
}
</script>

<style scoped>
.post{
    display: flex;
}
img {
    width: 440px;
    height: 270px;
    background-color: #6E38F7;
}
a{
    float: right;
}
.dateAndA{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    margin: 0 40px 10px;
}
h4{
    width: 460px;
    margin: 0 40px;
}
.postText{
    width: 460px;
    margin: 20px 40px;
    max-height: 132px;
    overflow: auto;
}
.content{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    padding: 20px;
    height: 270px;
}
</style>