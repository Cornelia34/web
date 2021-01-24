<template>
    <div>
        <div class="photoContainer">
            <link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.5.2/animate.min.css"/>
            <div class="photoContainerTitle animated fadeIn" style="animation-duration:3s;
            animation-iteration-count:1">國立清華大學藝術學院</div>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
    };
  },
};
</script>

<style lang="sass">
    .topContainer
        width:1140px
        height: 30px
        margin: auto
        background-color: #5A5757
    .topContainerContent
        font-size: 14px
        letter-spacing: 6.5px
        color: #FCFAF8
        text-aligen: justify
        padding-top: 6px
    .photoContainer
        //width:1400px
        margin: auto
        height: 100%
        background-image: url("https://scontent.ftpe7-2.fna.fbcdn.net/v/t1.0-9/140594558_789589164961744_8270012232425613214_o.jpg?_nc_cat=109&ccb=2&_nc_sid=730e14&_nc_ohc=ts3r95E92ggAX-nH6j2&_nc_ht=scontent.ftpe7-2.fna&oh=f28b6e4a61fb828b2c2d4400f3bcd39b&oe=602E5D85")
        //background-size: cover //不會重複
        //background-position: 0px -250px
        background-repeat: no-repeat
        background-attachment: fixed
        background-position: center
        background-size: cover
    .photoContainerTitle
        font-size: 36px
        color: #F7F3F0
        text-shadow: black 0.1em 0.1em 0.2em
        font-weight: 550
        letter-spacing: 25px
        padding: 275px
</style>
