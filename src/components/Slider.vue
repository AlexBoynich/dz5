<template>
    <section class="container">
        <h2>My social networks</h2>
    <p class="small-paragraph">There are many reasons to get down and start to get depressed about your situation. </p>
        <div>
        <a>&lt</a>
                <div id="items">
                <img src="@/assets/free-icon-instagram-2111463.png" class="item" alt="">
                <img src="@/assets/free-icon-odnoklassniki-3670250.png" class="item" alt="" >
                <img src="@/assets/free-icon-telegram-4401433.png" class="item" alt="">
                <img src="@/assets/free-icon-twitter-220375.png" class="item" alt="" >
                <img src="@/assets/free-icon-viber-3670059.png" class="item" alt="" >
                <img src="@/assets/free-icon-vkontakte-4494490.png" class="item" alt="" >
                <img src="@/assets/free-icon-whatsapp-4494494.png" class="item" alt="">
                <img src="@/assets/free-icon-youtube-4494485.png" class="item" alt="">
            </div>
        <a>></a>
         </div>
    </section>
</template>

<script>
export default{

}

</script>

<style scoped>
    section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    img{
        width:140px;
        height:80px;
        padding: 10px;
    }
    #items{
        max-width:100%;
        overflow: hidden;
        display: flex;
        margin-top: 20px;
    }
    h2{
        margin-top: 100px;
    }
    p{
        margin-top: 40px;
    }
    @media (max-width: 920px) {
        .container{
            padding-left:0;
            padding-right: 0;
        }
        div{
            max-width: 100%;
            display: flex;
            align-items: center;
        }
        h2{
            margin-top:50px;
        }
        .items{
            max-width:100px;
            max-height: 100px;
        }
    }
</style>