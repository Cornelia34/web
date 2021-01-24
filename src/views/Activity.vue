<template lang="pug">
    #app
        link(rel='stylesheet' type='text/css' href='https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.5.2/animate.min.css')
        .bigContainer
            .flexContainer
                .left
                    .left1Container
                        .left1TitleContainer
                            .left1TitleTitle 活動分類
                            ul.drop-down-menu
                                li
                                    a(href='#') 榮譽榜
                                        ul
                                            li
                                                a(href='#') 藝術學院教師獲獎
                                            li
                                                a(href='#') 春之獎學金
                                            li
                                                a(href='#') 春之卓越獎
                                            li
                                                a(href='#') 藝設系學生獲獎
                                            li
                                                a(href='#') 音樂系學生獲獎
                                            li
                                                a(href='#') 學士班學生獲獎
                                li
                                    a(href='#') 活動花絮
                                        ul
                                            li
                                                a(href='#') 藝院藝術季
                                            li
                                                a(href='#') 國際交流
                                li
                                    a(href='#') 藝術學報
                                        ul
                                            li
                                                a(href='#') 學報簡介
                                            li
                                                a(href='#') 編輯陣容
                                            li
                                                a(href='#') 徵稿須知
                                            li
                                                a(href='#') 文件下載
                .right
                    .right1Container
                        .right1PhotoContainer
                        .right1ContentContainer
                            .right1Title 榮譽榜
                            .right1Item(v-for="(item,id) in right1")
                                    .right1Content {{item.content}}
                    .right2Container
                        .right2ContentContainer
                            .right2Title 活動花絮
                            .right2Content {{right2}}
                        .right2PhotoContainer
                    .right3Container
                        .right3PhotoContainer
                        .right3ContentContainer
                            .right3Title 藝術學報
                            .right3Content {{right3}}
</template>

<script>
export default {
  data() {
    return {
      right1: [
        { content: '「2017新一代設計展」金點新秀設計獎 (工藝設計類)' },
        { content: '作品名稱：與貓的日常對話' },
        { content: '作者：藝設系陳婉宜' },
        { content: '作品簡介：互動是？在我的理解下互動是為對方的行為作出回應。寵物與人之間的關係應該是雙向的。動物與人類一來一往的遊戲，如同生活中的各種對話與回應。貓因為站立的位置不同而使貓屋傾斜或旋轉，就像是對人類作出回應一般。' },
      ],
      right2: '106年5月藝術學院於桃竹苗地區舉辦「2017第五屆國際臺灣客家文化藝術季」共計11場之系列活動，活動內容包含客家文化資源展、客家舞蹈展演、研討會、戲劇演出、文創商品展覽及音樂會演出活動，還邀請了多位國際級的音樂家參與演出：國際小提琴大師林昭亮先生、有「木笛界帕格尼尼」美稱的知名瑞士籍木笛演奏家Maurice Steger、意大利籍長笛家Rita D’Arcangelo、來自施洛維尼亞的手風琴家Primoz Parovel、美籍臺裔小提琴家林士凱、德籍臺裔長笛家劉士誠與築夢舞集等。',
      right3: '因合校因素，《新竹教育大學人文社會學報》自106年1月起停刊，轉型後刊物更名為《清華藝術學報》，改由本校藝術學院發行，歡迎美術、工藝、設計、美學文化思潮、策展、藝評、藝術行政管理、電影、音樂、其他表演藝術及藝術跨域研究相關論文投稿。',
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
.left1Item
    width: 213px
    height: 25px
    margin-bottom: 15px
    //border: 1px green solid

ul
  /* 取消ul預設的內縮及樣式
  margin: 5px
  padding: 0px
  list-style: none
  &.drop-down-menu
    //border: #ccc 1px solid
    display: inline-block
    font-size: 12px
    letter-spacing: 3px
    //color: #5B5350
    li
      position: relative
      white-space: nowrap
      //border-right: #ccc 1px solid
    > li
      &:last-child
        border-right: none
        float: center  //第一層對齊
    a
      background-color: #EBEBEB
      color: #5B5350
      display: block
      padding: 0 30px
      text-decoration: none
      line-height: 40px
      &:hover
        /* 滑鼠滑入按鈕變色
        background-color: #5A5757
        color: #EBEBEB
      &:hover > ul
          display: block
    li:hover > a
      /* 滑鼠移入次選單上層按鈕保持變色
      background-color: #5A5757
      color: #EBEBEB
    ul
      border: #CFCBC9 1px solid
      position: absolute
      z-index: 99
      left: 100px
      top: 0%
      min-width: 180px
      li
        //border-bottom: #ccc 1px solid
        &:last-child
            border-bottom: none
      /*隱藏次選單
      display: none

.right
    width: 810px
    height: 1160px
    //border: black 1px solid
    padding: 40px

.right1Container
    width: 805px
    height: 300px
    //border: red 1px solid
    margin-bottom: 40px
    display: flex
.right1ContentContainer
    width: 355px
    height: 300px
    //border: red 1px solid
.right1Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right1Content
    font-size: 13px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
    line-height: 20px
.right1PhotoContainer
    width: 450px
    height: 320px
    background-image: url("https://scontent.ftpe8-3.fna.fbcdn.net/v/t1.0-9/142508017_227237315726692_3227335418996124369_n.jpg?_nc_cat=106&ccb=2&_nc_sid=730e14&_nc_ohc=FxYgWKxdJ3QAX8BHkyt&_nc_ht=scontent.ftpe8-3.fna&oh=142b54503bc97d9441abaa9916c9253c&oe=60322973")
    background-size: 450px
    background-repeat: no-repeat

.right2Container
    width: 805px
    height: 300px
    //border: red 1px solid
    margin-bottom: 40px
    display: flex
.right2ContentContainer
    width: 355px
    height: 300px
    //border: red 1px solid
.right2Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right2Content
    font-size: 13px
    letter-spacing: 4px
    color: #5B5350
    text-align: left
    padding: 5px
    text-indent:2em
    line-height: 20px
.right2PhotoContainer
    width: 450px
    height: 320px
    background-image: url("https://art.nthu.edu.tw/wp-content/uploads/2017/09/2017-09_intl-01.jpg")
    background-size: 450px
    background-repeat: no-repeat

.right3Container
    width: 805px
    height: 300px
    //border: red 1px solid
    margin-bottom: 40px
    display: flex
.right3ContentContainer
    width: 355px
    height: 300px
    //border: red 1px solid
.right3Title
    font-size: 18px
    font-weight: 550
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px
.right3Content
    font-size: 13px
    letter-spacing: 3px
    color: #5B5350
    text-align: left
    padding: 5px 7px
    text-indent:2em
    line-height: 20px
.right3PhotoContainer
    width: 450px
    height: 320px
    background-image: url("https://images.pexels.com/photos/6214/hands-people-woman-girl.jpg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940")
    background-size: 450px
    background-repeat: no-repeat
</style>>
