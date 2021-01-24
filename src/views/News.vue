<template lang="pug">
#app
    .bigContainer
        .flexContainer
            .left
                .left1Container
                    //iframe(src='https://calendar.google.com/calendar/embed?height=250&wkst=1&bgcolor=%23ffffff&ctz=Asia%2FTaipei&src=ZjBvdHUwMDFwYXZuc2Q3OW84MTY1b2Fpb2tAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ&color=%23EF6C00&showPrint=0&showTz=0&showNav=0&showTitle=0&showTabs=0&showCalendars=0' style='border:solid 1px #777' width='235' height='250' frameborder='0' scrolling='no')
                    h3 January 2021
                    ol.calendar
                        li.day-name Sun
                        li.day-name Mon
                        li.day-name Tue
                        li.day-name Wed
                        li.day-name Thu
                        li.day-name Fri
                        li.day-name Sat
                        li.first-day 1
                        li 2
                        li 3
                        li 4
                        li 5
                        li 6
                        li 7
                        li 8
                        li 9
                        li 10
                        li 11
                        li 12
                        li 13
                        li 14
                        li 15
                        li 16
                        li 17
                        li 18
                        li 19
                        li 20
                        li 21
                        li 22
                        li 23
                        li 24
                        li 25
                        li 26
                        li 27
                        li 28
                        li 29
                        li 30
                        li 31
                .left2Container
                    .left2TitleContainer
                        .left2TitleTitle 近期文章
                    .left2FlexContainer
                        .left2Flex
                            .left2Item(v-for="(item,id) in left2" :class="id%2==0? 'left2color1':'left2color2'")
                                .left2Text
                                    .left2Content {{item.content}}
                .left3Container
                    .left3TitleContainer
                        .left3TitleTitle 文章分類
                    .left3FlexContainer
                        .left3Item(v-for="(item,id) in left3")
                                .left3Text
                                    .left3Content {{item.content}}
            .right
                .right1Container
                    .right1PhotoContainer
                    .right1ContentContainer
                        .right1Date 20210107
                        .right1Title 《徵才》國立清華大學藝術學院誠徵專題計畫約用人員1名
                        .right1Content 國立清華大學藝術學院誠徵專題計畫約用人員1名 聘任單位：國立清華大學藝術學院...
                        .Readmore Readmore
                .right2Container
                    .right2ContentContainer
                        .right2Date 20201208
                        .right2Title 藝設系學生獲獎：109年林務局「國產材設計商品比賽」決選
                        .right2Content 藝設系工藝設計組研究生魏嘉琪 獲109年由林務局舉辦之「國產材商品設計比賽」...
                        .Readmore Readmore
                    .right2PhotoContainer
                .right3Container
                    .right3PhotoContainer
                    .right3ContentContainer
                        .right3Date 20201201
                        .right3Title 2021藝術學院教育發展基金
                        .right3Content
                            a(href='https://art.nthu.edu.tw/wp-content/uploads/2020/12/2021%E5%B9%B4%E7%99%BC%E5%B1%95%E5%9F%BA%E9%87%91-%E8%97%9D%E8%A1%93%E5%AD%B8%E9%99%A21091120.pdf' target="_blank") 2021年發展基金–藝術學院1091120
                .right4Container
                    .right4ContentContainer
                        .right4Date 20201201
                        .right4Title 《開放報名》2020國立清華大學藝設系研究生論文研討會
                        .right4Content 2020國立清華大學藝術與設計學系研究生論文研討會 開放報名 報名網址：...
                        .Readmore Readmore
                    .right4PhotoContainer
</template>

<script>
export default {
  data() {
    return {
      left2: [
        { content: '《徵才》國立清華大學藝術學院誠徵專題計畫約用人員1名' },
        { content: '藝設系學生獲獎：109年林務局「國產材設計商品比賽」決選' },
        { content: '2021藝術學院教育發展基金' },
        { content: '《開放報名》2020國立清華大學藝設系研究生論文研討會' },
        { content: '清華大學藝設系研究生論文研討會：徵稿' },
        { content: 'ARS 2020 – Tsing Hua Garden' },
        { content: '清華藝術學報' },
        { content: '藝設系設計組-異質對話-（360展區1）' },
        { content: '華山烏梅劇場"Face to face"實驗性跨領域展演' },
      ],
      left3: [
        { content: 'Top news' },
        { content: '合作交流' },
        { content: '國際交流' },
        { content: '學生獲獎' },
        { content: '學院公告' },
        { content: '學院活動' },
        { content: '招生訊息' },
      ],
    };
  },
};
</script>
<style lang="sass">
a
    color: #7E678E
    text-decoration: none
.bigContainer
    weight: 1400px
    height: 1600px
    background-color: #5A5757
    position: relative
    padding-top: 20px
.flexContainer
    width: 1150px
    height: 1500px
    margin: auto
    background-color: #EBEBEB
    position: relative
    display: flex
    //flex-wrap: wrap
.left
    width: 240px
    height: 1350px
    //border: black 1px solid
    padding: 40px 10px 40px
.right
    width: 810px
    height: 1350px
    //border: black 1px solid
    padding: 40px

.left1Container
    width: 235px
    height: 230px
    //border: red 1px solid
    position: relative
    margin-bottom: 15px
    font: 100% system-ui
    font-size: 14px

.calendar
    display: grid
    grid-template-columns: repeat(7, 1fr)
.first-day
    grid-column-start: 6
.day-name
    color: #5A5757
    background: #CFCBC9
h3
    text-align: center
ol
    list-style: none
    margin: 0
    padding: 0
    text-align: center
li
    padding: 1px

.left2Container
    width: 225px
    height: 425px
    //border: red 1px solid
    position: relative
    margin-bottom: 15px
    padding: 10px 5px 10px
.left2TitleContainer
    width: 180px
    height: 30px
    margin: 0px 20px 10px
    position: relative
    background-color: #5A5757
.left2TitleTitle
    font-size: 18px
    letter-spacing: 5px
    text-align: center
    color: #EBEBEB
    padding: 3px
.left2FlexContainer
    width: 213px
    height: 387px
    margin: 0px 5px 10px
    position: relative
    //border: red 1px solid
.left2Flex
    display: flex //排列方式
    flex-direction: column
    justify-content: flex-start
    flex-wrap: wrap
.left2Item
    width: 213px
    height: 34px
    margin-bottom: 10px
    //padding: 10px 5px //上下 左右
    //background-color: #C4D7D1
    //text-align: left
    //display: flex
    //flex-direction: column
    //justify-content: flex-start
.left2color1
    background-color: #CFCBC9 //待改
.left2color2
    background-color: #C4D7D1
.left2Content
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding-left: 2px

.left3Container
    width: 225px
    height: 425px
    //border: red 1px solid
    position: relative
    margin-bottom: 15px
    padding: 10px 5px 10px
.left3TitleContainer
    width: 180px
    height: 30px
    margin: 0px 20px 10px
    position: relative
    background-color: #5A5757
.left3TitleTitle
    font-size: 18px
    letter-spacing: 5px
    text-align: center
    color: #EBEBEB
    padding: 3px
.left3FlexContainer
    width: 213px
    height: 387px
    margin: 0px 5px 10px
    position: relative
    //border: red 1px solid
.left3Flex
    display: flex //排列方式
    flex-direction: column
    justify-content: flex-start
    flex-wrap: wrap
.left3Item
    width: 213px
    height: 25px
    margin-bottom: 15px
    //border: 1px green solid
.left3Content
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: center
    padding: 4px 2px 4px

.right1Container
    width: 805px
    height: 320px
    //border: red 1px solid
    position: relative
    margin-bottom: 40px
    display: flex
.right1PhotoContainer
    width: 305px
    height: 320px
    background-image: url("https://icon-library.com/images/recruiting-icon/recruiting-icon-18.jpg")
    background-size: 305px
.right1ContentContainer
    width: 500px
    height: 320px
    //border: red 1px solid
.right1Date
    font-size: 12px
    font-family: Verdana
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right1Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right1Content
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.Readmore
    font-size: 12px
    font-family: Verdana
    letter-spacing: 3px
    color: #5B5350
    text-align: right
    padding: 170px 10px 5px

.right2Container
    width: 805px
    height: 320px
    //border: red 1px solid
    position: relative
    margin-bottom: 40px
    display: flex
.right2ContentContainer
    width: 500px
    height: 320px
    //border: red 1px solid
.right2Date
    font-size: 12px
    font-family: Verdana
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
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
.right2PhotoContainer
    width: 305px
    height: 320px
    background-image: url("https://art.nthu.edu.tw/wp-content/uploads/2020/12/%E6%8B%9A%E5%8D%A1.jpg")
    background-size: 305px

.right3Container
    width: 805px
    height: 320px
    //border: red 1px solid
    position: relative
    margin-bottom: 0px
    display: flex
.right3PhotoContainer
    width: 305px
    height: 320px
    background-image: url("https://toppng.com/uploads/preview/uzyskaj-gotowke-icon-fund-icon-11553485402oxnw4rliad.png")
    background-size: 305px
.right3ContentContainer
    width: 500px
    height: 320px
    //border: red 1px solid
.right3Date
    font-size: 12px
    font-family: Verdana
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right3Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right3Content
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px

.right4Container
    width: 805px
    height: 320px
    //border: red 1px solid
    position: relative
    display: flex
.right4ContentContainer
    width: 500px
    height: 320px
    //border: red 1px solid
.right4Date
    font-size: 12px
    font-family: Verdana
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right4Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right4Content
    font-size: 12px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right4PhotoContainer
    width: 305px
    height: 320px
    background-image: url("https://art.nthu.edu.tw/wp-content/uploads/2020/12/%E5%BE%B5%E7%A8%BF%E6%B5%B7%E5%A0%B1-768x1086.jpg")
    background-size: 305px
</style>
