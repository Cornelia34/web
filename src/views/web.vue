<<<<<<< HEAD
<!-- eslint-disable max-len -->

=======
>>>>>>> 21cf42510947c09c4f6bbfd263cb9f1c30d60dcc
<template lang="pug">
#app
    .topContainer
        .topContainerContent {{topContent}}
    .searchContainer
        .searchContainerContent Search
    .searchPhotoContainer
    .photoContainer
        .photoContainerTitle {{photoTitle}}
        //img.photo(v-bind:src="img" width="1140px")
    .bottomContainer
        .bottomContainerContent {{bottomContent}}
    .newsContainer
        .newsPageTitle {{newsTitle}}
        .newsFlex
            .newsItem(v-for="(item,id) in news" :class="id%2==0? 'dark':'light'")
                .newsText
                    .newsDate {{item.date}}
                    .newsTitle {{item.title}}
                    .newsContent {{item.content}}
                .readMore Read More
        .newsPageBottomFlex
            .newsPageBottomItem(v-for="(item,id) in newsBottom" :class="id%2==0? 'content1':'content2'")
                .newsPageBottomContent {{item.content}}
    .IPTAphotoContainer
    .welcomeContainer
        .welcomeFlex
            .welcomeItem(v-for="item in welcome")
                .welcomeText
                    .welcomeTitle {{item.title}}
                    .welcomeContent {{item.content}}
    .webTitleContainer
        .webTitleTitle 學院相關網站
    .webContainer
        .webFlex
            .webItem(v-for="(item,id) in web" :class="id%2==0? 'dark2':'light2'")
                .webText
                    .webContent {{item.content}}

</template>

<script>
export default {
  data() {
    return {
      topContent: 'HOME 關於學院 學院師資 學院規章 招生訊息 榮譽榜 活動花絮 藝院影音 藝術學院 聯絡資訊',
      photoTitle: '國立清華大學藝術學院',
      bottomContent: 'Facebook Twitter E-mail TEL:+886-3-5715131#78801',
      newsTitle: 'News',
      // img: 'https://drive.google.com/file/d/1DVGm7dgfd1fYBvbX3qYlFKWY5BY7qdoV/view?usp=sharing',
      news: [
        { date: '20201208', title: '藝設系學生獲獎－109年林務局「國產材設計商品比賽」決選', content: '藝設系工藝設計組研究生魏嘉琪 獲109年由林務局舉辦之「國產材商品設計比賽」......' },
        { date: '20201201', title: '2021 年藝術學院教育發展基金', content: '2021年發展基金–藝術學院1091120 ' },
        { date: '20201201', title: '【開放報名】2020國立清華大學藝術與設計學系研究生論文研討會', content: '2020國立清華大學藝術與設計學系研究生論文研討會 開放報名 報名網址......' },
        { date: '20200924', title: '清華大學藝設系研究生論文研討會 – 徵稿', content: '' },
<<<<<<< HEAD
        { date: '20200909', title: 'ARS 2020 – Tsing Hua Garden', content: '今年全球最大的科技藝術節 – 奧地利林茲的〝國際電子藝術節......' },
=======
        { date: '20200909', title: 'ARS 2020 – Tsing Hua Garden', content: '今年全球最大的科技藝術節 – 奧地利林茲的〝國際電子藝術節......'}
>>>>>>> 21cf42510947c09c4f6bbfd263cb9f1c30d60dcc
      ],
      newsBottom: [
        { content: '《《' },
        { content: '》》' },
      ],
      welcome: [
<<<<<<< HEAD
        { title: '院學士班招生 科技藝術！', content: '歡迎你一起來開創清華科技藝術跨域DNA！' },
        { title: '藝設系招生 「藝」鳴驚人！', content: '歡迎你一起來把美感、創意帶入清華生活！' },
        { title: '音樂系招生 全方位音樂人！', content: '歡迎你一起在清華創造音樂心靈饗宴！' },
=======
        { title: '院學士班招生 科技藝術！', content: '歡迎你一起來開創清華科技藝術跨域DNA！'},
        { title: '藝設系招生 「藝」鳴驚人！', content: '歡迎你一起來把美感、創意帶入清華生活！'},
        { title: '音樂系招生 全方位音樂人！', content: '歡迎你一起在清華創造音樂心靈饗宴！'},
>>>>>>> 21cf42510947c09c4f6bbfd263cb9f1c30d60dcc
      ],
      web: [
        { content: '藝設系' },
        { content: '音樂系' },
        { content: '院學士班' },
        { content: '藝術科技碩班' },
        { content: '春之藝術專題講座' },
<<<<<<< HEAD
        { content: '科技藝術研究中心' },
=======
        { content: '科技藝術研究中心'},
>>>>>>> 21cf42510947c09c4f6bbfd263cb9f1c30d60dcc
      ],
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
    .searchContainer
        width: 153px
        height: 18px
        border-radius: 18px
        background-color: #FCFCFC
        position: absolute
        margin-top: 8px
        right: 50px
    .searchContainerContent
        text-align: right
        color: #5A5757
        font-size: 12px
        font-family: Verdana
        padding: 1px
        padding-right: 20px
        letter-spacing: 2px
    .searchPhotoContainer
        //border: 1px solid #AAA
        width: 18px
        height: 18px
        border-radius: 18px
        //background-color: #FCFC
        background-image: url("//upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Search_Noun_project_15028.svg/47px-Search_Noun_project_15028.svg.png")
        background-size: cover //不會重複
        position: absolute
        margin-top: 8px
        right: 50px
    .photoContainer
        width:1140px
        margin: auto
        height: 460px
        background-image: url("https://scontent.ftpe7-4.fna.fbcdn.net/v/t1.0-9/132044625_771682910085703_8650818129536171912_o.jpg?_nc_cat=105&ccb=2&_nc_sid=730e14&_nc_ohc=9wap0dM0YeUAX-JSptB&_nc_ht=scontent.ftpe7-4.fna&oh=b8b57123989948ab80bf23306f537649&oe=60049A86")
        background-size: cover //不會重複
        background-position: 0px -180px
    .photoContainerTitle
        font-size: 36px
        color: #F7F3F0
        text-shadow: black 0.1em 0.1em 0.2em
        font-weight: 550
        letter-spacing: 25px
        padding-top: 202px
    .bottomContainer
        width:1140px
        height: 30px
        margin: auto
        background-color: #5A5757
        margin-bottom: 20px
    .bottomContainerContent
        font-size: 14px
        letter-spacing: 6px
        color: #FCFAF8
        font-family: Verdana
        text-aligen: inter-ideograph
        padding-top: 7px
    .newsContainer
        width:1140px
        margin: auto
        height: 405px
        background-image: url("https://thumbs.dreamstime.com/z/hand-drawn-simple-watercolor-pattern-background-circles-white-125973170.jpg")
        backgroung-size: cover
        background-position: -350px -375px
        margin-bottom: 20px
    .newsPageTitle
        text-align: right
        font-size: 30px
        letter-spacing: 3px
        font-weight: 550
        font-family: Palatino
    //flex css
    .newsFlex
        display: flex //排列方式
        flex-direction: row
        justify-content: space-between
        flex-wrap: wrap
    .newsItem
        width: 200px
        height: 320px
        padding: 10px 10px //上下 左右
        text-align: left
        display: flex
        flex-direction: column
        justify-content: space-between
    .dark
        background-color: #FFB7A1
    .light
        background-color: #F5D1C3
    .newsDate
        font-size: 14px
        letter-spacing: 3px //字距
        margin-bottom: 5px
        //font-weight: 550 //加粗
        font-family: Verdana
    .newsTitle
        font-size: 18px
        letter-spacing: 2px
        margin-bottom: 5px
        font-weight: 700
        text-align: justify
    .newsContent
        font-size: 14px
        letter-spacing: 2px
        color: #5B5350
        text-align: justify
        text-indent: 2em
    .readMore
        font-size: 15px
        letter-spacing: 2.5px
        text-align: right
        font-family: Palatino
        font-weight: 550
    .newsPageBottomFlex
        display: flex //排列方式
        flex-direction: row
        justify-content: space-between
        flex-wrap: wrap
    .newsPageBottomItem
        width: 30px
        height: 30px
        display: flex
        flex-direction: column
        justify-content: space-between
        //border: 1px solid #AAA
    .content1
        text-align: left
        font-size: 20px
        letter-spacing: -8px
        font-weight: 550
    .content2
        text-align: right
        font-size: 20px
        letter-spacing: -8px
        font-weight: 550
    .IPTAphotoContainer
        width:1140px
        margin: auto
        height: 350px
        //border: 1px solid #AAA
        background-image: url("http://ipta.nthu.edu.tw/wp-content/uploads/2020/10/poster_web.png")
        backgroung-size: cover
        background-position: -50px -495px
        border-radius: 50px
        margin-bottom: 5px
    .welcomeContainer
        width:1140px
        margin: auto
        height: 175px
        //border: 1px solid #AAA
        margin-bottom: 20px
    .welcomeFlex
        display: flex //排列方式
        flex-direction: row
        justify-content: space-between
        flex-wrap: wrap
    .welcomeItem
        width: 330px
        height: 150px
        padding: 10px 5px //上下 左右
        background-color: #FFB7A1
        border-radius: 20px
        text-align: left
        display: flex
        flex-direction: column
        justify-content: space-between
    .welcomeTitle
        font-size: 18px
        letter-spacing: 1.5px
        margin-bottom: 3px
        font-weight: 700
        text-align: center
        padding-top: 45.5px
    .welcomeContent
        font-size: 14px
        letter-spacing: 2.5px
        color:  #5B5350
        text-align: center
    .webTitleContainer
        width:235px
        margin: auto
        height: 25px
        background-color: #5A5757
        margin-bottom: 5px
    .webTitleTitle
        font-size: 14px
        letter-spacing: 5px
        text-align: center
        color: #F7F3F0
        padding: 1.75px
    .webContainer
        width:750px
        margin: auto
        height: 120px
    .webFlex
        display: flex //排列方式
        flex-direction: row
        justify-content: space-between
        flex-wrap: wrap
    .webItem
        width: 100px
        height: 100px
        padding: 10px 5px //上下 左右
        background-color: #C4D7D1
        text-align: left
        display: flex
        flex-direction: column
        justify-content: space-between
    .dark2
        background-color: #AAB8BB
    .light2
        background-color: #C4D7D1
    .webContent
        font-size: 12px
        letter-spacing: 3px
        color: #5B5350
        text-align: center
        padding: 36px 15px
</style>
