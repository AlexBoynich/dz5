<template>
    <section class="form container">
        <h2 id="contact">Contact us</h2>
        <p class="small-paragraph">Life is 10% what happens to you and 90% how you react to it. It does not matter how slowly you go as long as you do not stop. Confucius.</p>
        <form class="form">
            <div class="name-email">
                <input class="name inputs" type="text" size="40" placeholder="Your name">
                <input class="email inputs" type="text" size="40" placeholder="Email">
            </div>
                <textarea class="description inputs" name="description" cols="40" rows="3" placeholder="Description (optional)"></textarea>
                <button class="button inputs">SEND</button>
            </form>
    </section>
</template>

<script>
import Button from './Button.vue';
import Inputs from './Inputs.vue';

    export default {
        props:['buttonProps'],
            components: {
                Button,
                Inputs
            }
    }
</script>

<style>
.form{
    display: flex;
    flex-direction: column;
    align-items: center;
}
input, textarea{
    display: flex;
    border-radius: 4px;
    margin: 20px 10px 0;
    font-family: Rubik;
    font-size: 16px;
    font-weight: 400;
    line-height: 22px;
    letter-spacing: 0px;
    text-align:start;
    border: 1px solid #CAD1E1;
    padding: 12px 15px;
    box-sizing: border-box;
}
.name-email{
    display: flex;
    flex-direction: row;
}
input {
    width: 218px;
}
textarea{
    width: 460px;
    height: 122px;
}
button{
    display: flex;
    width: 160px;
    height: 46px;
    font-family: Rubik;
    font-size: 16px;
    font-weight: 400;
    line-height: 22px;
    letter-spacing: 0px;
    background-color: #6E38F7;
    align-items: center;
    justify-content: center;
    color: #ffffff;
    font-size: 12px;
    margin-top: 30px;
    margin-bottom: 100px;
    border-radius: 4px;
}

@media (max-width: 920px) {
    .name-email{
        flex-direction: column;
    }
    input{
        width: 288px;
        height: 46px;
    }
    textarea{
        width: 288px;
        height: 122px;
    }
    button{
        width: 288px;
        height: 46px;
        margin-bottom: 60px;
    }
}
</style>