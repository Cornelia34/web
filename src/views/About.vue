<template>
  <div class="bigContainer">
    <div class="slider_container">
      <div>
          <img src="https://scontent.ftpe7-3.fna.fbcdn.net/v/t1.0-9/140320132_789589214961739_3433143602067764208_o.jpg?_nc_cat=102&ccb=2&_nc_sid=730e14&_nc_ohc=2-8Yc52zujIAX8dCR1T&_nc_ht=scontent.ftpe7-3.fna&oh=f17492db8c51e71f8c8624da48fc7a0f&oe=602E1EA1" width="1000" alt="pure css3 slider" />
          <span class="info">TechArt</span>
      </div>
      <div>
          <img src="https://scontent.ftpe7-2.fna.fbcdn.net/v/t1.0-9/140627181_789589221628405_9095097256592353256_o.jpg?_nc_cat=109&ccb=2&_nc_sid=730e14&_nc_ohc=py5JZZPLenMAX_Yf4YI&_nc_ht=scontent.ftpe7-2.fna&oh=ec59492e28c998fbe7b3a9c7229ad3bd&oe=602DC7D6" width="1000" alt="pure css3 slider"/>
          <span class="info">Musical Performing</span>
      </div>
      <div>
          <img src="https://scontent.ftpe7-1.fna.fbcdn.net/v/t1.0-9/141449154_789589151628412_2786300556555511278_o.jpg?_nc_cat=100&ccb=2&_nc_sid=730e14&_nc_ohc=Y5eX9wOvvNYAX-FSZHO&_nc_ht=scontent.ftpe7-1.fna&oh=0f700f9ae88a4d5e582c20486b4d92d4&oe=602F7E89" width="1000" alt="pure css3 slider" />
          <span class="info">Sculpting</span>
      </div>
      <div>
          <img src="https://scontent.ftpe7-1.fna.fbcdn.net/v/t1.0-9/140657717_789589158295078_8699330637508521297_o.jpg?_nc_cat=100&ccb=2&_nc_sid=730e14&_nc_ohc=UKQ5UIrv9rMAX_vB4so&_nc_ht=scontent.ftpe7-1.fna&oh=00a90c15385d3a88feb985342ed08253&oe=602DAF3D" width="1000" alt="pure css3 slider" />
          <span class="info">Painting</span>
      </div>
      <div>
          <img src="https://art.nthu.edu.tw/wp-content/uploads/2020/09/ARS2020-1.jpg" width="1025" alt="pure css3 slider" />
          <span class="info">ARS 2020 – Tsing Hua Garden</span>
      </div>
    </div>
    <div class="PDContainer">
        <div class="PDFlex">
          <div id="PDItem-1"></div>
          <div id="PDItem-2">
            <a href="http://artdesign.site.nthu.edu.tw/?Lang=zh-tw" target="_blank">藝術與設計學系</a>
            <br> 歡迎你一起來把美感、創意帶入清華生活！</div>
        </div>
    </div>
    <div class="musicContainer">
      <div class="musicFlex">
        <div id="musicItem-1">
          <a href="http://music.site.nthu.edu.tw/?Lang=zh-tw" target="_blank">音樂學系</a>
          <br> 歡迎你一起在清華創造音樂心靈饗宴！</div>
        <div id="musicItem-2"></div>
      </div>
    </div>
    <div class="TAContainer">
      <div class="TAFlex">
        <div id="TAItem-1"></div>
        <div id="TAItem-2"><a href="http://ipta.nthu.edu.tw/" target="_blank">藝術學院學士班</a>
        <br> 歡迎你一起來開創清華科技藝術跨域DNA！</div>
      </div>
    </div>
  </div>
</template>

<style lang="sass">
    a
      color: #7E678E
      text-decoration: none
    .bigContainer
        weight: 1400px
        height: 2250px
        background-color: #5A5757
        position: relative
        padding-top: 20px
    .slider_container
        margin: auto
        width: 1050px
        height: 705px
        position: relative
        background-color: #EBEBEB
        margin-bottom: 20px
        border-radius: 20px

    .slider_container div
        padding-top: 10px
        position: absolute
        top: 0
        left: 0
        opacity: 0
        filter: alpha(opacity=0)

    .slider_container div
        -webkit-animation: round 25s linear infinite
        animation: round 25s linear infinite

    @-webkit-keyframes round
        4%
            opacity: 1
            filter: alpha(opacity=100)
            /* 0 - 1秒 淡入*/
        20%
            opacity: 1
            filter: alpha(opacity=100)
            /* 1- 5秒靜止*/
        24%
            opacity: 0
            filter: alpha(opacity=0)
            /* 5-6秒淡出*/

    @keyframes round
        4%
            opacity: 1
            filter: alpha(opacity=100)
            /* 0 - 1秒 淡入*/
        20%
            opacity: 1
            ilter: alpha(opacity=100)
            /* 1- 5秒靜止*/
        24%
            opacity: 0
            filter: alpha(opacity=0)
            /* 5-6秒淡出*/

    .slider_container div:nth-child(5)
        -webkit-animation-delay: 0s
        animation-delay: 0s
    .slider_container div:nth-child(4)
        -webkit-animation-delay: 5s
        animation-delay: 5s
    .slider_container div:nth-child(3)
        -webkit-animation-delay: 10s
        animation-delay: 10s
    .slider_container div:nth-child(2)
        -webkit-animation-delay: 15s
        animation-delay: 15s
    .slider_container div:nth-child(1)
        -webkit-animation-delay: 20s
        animation-delay: 20s

    .PDContainer
        width: 1150px
        height: 405px
        margin: auto
        background-color: #EBEBEB
        position: relative
        margin-bottom: 20px
        padding-top: 55px

    .PDFlex
        display: flex //排列方式
        width: 1000px
        height: 350px
        //outline: 1px green solid
        margin: auto
        position: relative
    #PDItem-1
      width: 600px
      //background-color: cyan
      background-image: url("https://scontent.ftpe7-3.fna.fbcdn.net/v/t1.0-9/139435664_789765714944089_5341190379935970669_o.jpg?_nc_cat=103&ccb=2&_nc_sid=730e14&_nc_ohc=TZhojFr6gXwAX8r3epo&_nc_ht=scontent.ftpe7-3.fna&oh=f407c5cc28e84c136d27ea6eb5babbcd&oe=602DD069")
      background-size: cover
    #PDItem-2
      width: 400px
      //background-color: #AAB8BB
      font-size: 18px
      letter-spacing: 2px
      margin:  100px 0px 100px 20px
      text-align: left
      padding-top: 55px
      color: #5A5757
      //font-weight: 550
      //line-height: 150px

    .musicContainer
        width: 1150px
        margin: auto
        height: 405px
        background-color: #EBEBEB
        position: relative
        margin-bottom: 20px
        padding-top: 55px
    .musicFlex
        display: flex //排列方式
        width: 1000px
        height: 350px
        margin: auto
        position: relative
    #musicItem-1
      width: 400px
      //background-color: cyan
      font-size: 18px
      letter-spacing: 2px
      margin:  100px 20px 100px 0px
      text-align: left
      padding-top: 55px
      color: #5A5757
    #musicItem-2
      width: 600px
      background-image: url("http://music.site.nthu.edu.tw/var/file/113/1113/img/336/192466575.jpg")
      background-size: cover //不會重複

    .TAContainer
        width: 1150px
        margin: auto
        height: 405px
        background-color: #EBEBEB
        position: relative
        margin-bottom: 20px
        padding-top: 55px
    .TAFlex
        display: flex //排列方式
        width: 1000px
        height: 350px
        margin: auto
        position: relative
    #TAItem-1
      width: 600px
      background-image: url("https://ipta.nthu.edu.tw/wp-content/uploads/2020/10/poster_web.png")
      background-size: cover //不會重複
      background-position: 0px -490px
    #TAItem-2
      width: 400px
      //background-color: khaki
      font-size: 18px
      letter-spacing: 2px
      margin:  100px 0px 100px 20px
      text-align: left
      padding-top: 55px
      color: #5A5757
</style>
