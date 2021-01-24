<template lang="pug">
    #app
        link(rel='stylesheet' type='text/css' href='https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.5.2/animate.min.css')
        .bigContainer
            .flexContainer
                .left
                    .left1Container
                        .left1TitleContainer
                            .left1TitleTitle 聯絡資訊
                        .left1FlexContainer
                            .left1Item(v-for="(item,id) in left1")
                                .left1Text
                                    .left1Content {{item.content}}
                .right
                    .right1PhotoContainer.animated.fadeIn
                    .right2ContentContainer
                        .right2Title 藝術學院
                        .right2Item(v-for="(item,id) in right1")
                            .right2Content {{item.content}}
                    .right3Container
                        .right3Item(v-for="(item,id) in right3")
                            .right3Title {{item.title}}
                            .right3TEL {{item.tel}}
                            .right3Other {{item.other}}
                            .right3Email {{item.email}}
</template>

<script>
export default {
  data() {
    return {
      left1: [
        { content: '藝術學院' },
        { content: '藝術設計學系' },
        { content: '音樂學系' },
        { content: '藝術學院學士班' },
      ],
      right1: [
        { content: '地址：30014新竹市南大路521號（清華南大校區行政大樓3F藝術學院）' },
        { content: '院秘書：吳淑宜小姐' },
        { content: 'Tel：+886-3-5715131 #78801或78802' },
        { content: 'Fax: +886-3-5619170' },
        { content: 'Email：coa@my.nthu.edu.tw' },
      ],
      right3: [
        { title: '藝術設計學系', tel: 'Tel：03-5715131 #72901、72903 ', other: 'Fax：03-5245209', email: 'Email：artist@my.nthu.edu.tw' },
        { title: '音樂學系', tel: 'Tel：03-5715131 #73101、73103、73104（系辦公室）', other: 'Fax：03-5245192', email: 'Email：dme@mail.nhcue.edu.tw' },
        { title: '藝術學院學士班', tel: 'Tel：03-5715131 #78802（系辦公室）', email: 'Email：cwyu@mx.nthu.edu.tw ' },
      ],
    };
  },
};

</script>

<style lang="sass">
.bigContainer
    weight: 1400px
    height: 1300px
    background-color: #5A5757
    position: relative
    padding-top: 20px
.flexContainer
    width: 1150px
    height: 1200px
    margin: auto
    background-color: #EBEBEB
    position: relative
    display: flex
.left
    width: 240px
    height: 1160px
    //border: black 1px solid
    padding: 40px 10px 40px
.left1Container
    width: 225px
    height: 425px
    //border: red 1px solid
    position: relative
    margin-bottom: 15px
    padding: 10px 5px 10px
.left1TitleContainer
    width: 180px
    height: 30px
    margin: 0px 20px 10px
    position: relative
    background-color: #5A5757
.left1TitleTitle
    font-size: 18px
    letter-spacing: 5px
    text-align: center
    color: #EBEBEB
    padding: 3px
.left1FlexContainer
    width: 213px
    height: 387px
    margin: 0px 5px 10px
    position: relative
    //border: red 1px solid
.left1Flex
    display: flex //排列方式
    flex-direction: column
    justify-content: flex-start
    flex-wrap: wrap
.left1Item
    width: 213px
    height: 25px
    margin-bottom: 15px
    //border: 1px green solid
.left1Content
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: center
    padding: 4px

.right
    width: 850px
    height: 1160px
    //border: black 1px solid
    padding: 40px
.right1PhotoContainer
    width: 810px
    height: 552px
    position: relative
    margin-bottom: 20px
    background-image: url("http://art.nthu.edu.tw/wp-content/uploads/2017/09/NTHU-map-02.jpg")
    background-size: 810px
    background-repeat: no-repeat
.right2ContentContainer
    width: 810px
    height: 165px
    //border: red 1px solid
    margin-bottom: 40px
.right2Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right2Content
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px

.right3Container
    width: 810px
    height: 270px
    //border: red 1px solid
    display: flex //排列方式
    flex-direction: row
    justify-content: space-between
.right3Item
    width: 360px
    height: 265px
    //border: red 1px solid
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    line-height: 25px
    padding: 2px 5px 2px
.right3Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 4px
    color: #5B5350
    text-align: left

</style>>
