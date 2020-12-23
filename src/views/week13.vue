<template>
  <div id="app">
    <div class="header">
      <img class="logo" src="https://ipta.nthu.edu.tw/wp-content/uploads/2019/02/cropped-NTHU-logo.png">
      <div class="cube1"></div>
        <p class="p3">HOME</p>
      <div class="cube2"></div>
        <p class="p4">最新消息</p>
      <div class="cube3"></div>
        <p class="p5">招生</p>
        <div class="polygon1"></div>
      <div class="cube4"></div>
        <p class="p6">學士班</p>
        <div class="polygon2"></div>
      <div class="cube5"></div>
        <p class="p7">師資</p>
        <div class="polygon3"></div>
      <div class="cube6"></div>
        <p class="p8">科藝賞析</p>
        <div class="polygon4"></div>
      <div class="cube7"></div>
        <p class="p9">聯絡</p>
      <img class="photo1" src="https://ipta.nthu.edu.tw/wp-content/uploads/2017/10/BG.jpg">
      <div class="circle2"></div>
        <div class="circle1">
          <p class="p1">國立清華大學<br>藝術學院</p>
          <p class="p2">ipth</p>
        </div>
    </div>
    <div class="section">
      <img class="photo2" src="https://ipta.nthu.edu.tw/wp-content/uploads/2017/10/BG.jpg">
      <div class="rectangle1"></div>
        <p class="p10">學士班特色<br>清華是國際頂尖科技大學，加上合校後的藝術學院，具備發展「科技藝術」的卓越條件。我們號召臺灣年輕一代的科技藝術學者專家，我們規劃有科技藝術跨域特別課程，並與業界合作推出創意跨域專題。你，不需猶豫，歡迎你的加入！</p>
      <div class="rectangle2"></div>
        <p class="p11">核心能力<br>社會關懷與品格實踐能力｜美感認知與經典欣賞能力｜自然感知與創新發想能力｜邏輯思辨與語文溝通能力｜國際觀點與在地行動能力｜資訊掌握與科技應用能力</p>
      <div class="rectangle3"></div>
        <p class="p12">清華大學2018年成立藝術學院〝科技藝術〞跨域「學士班」。「科技藝術（TechArt）」是當代藝術的新形式創作也是國際藝術發展的重要趨勢，包含虛擬藝術、互動藝術、電腦動畫、電腦音樂、聲音藝術、科技性表演藝術、混合藝術、網路社群、創客藝術、仿生藝術、生物藝術、人工生命…等。在當代數位美學與數位藝術的基礎下，我們結合創新科技，如各種互動感測技術、虛擬實境、物聯網、人工智慧、大數據分析、基因工程…，把「科技」與「藝術」結合視為「未來文化學」，培養前瞻性、跨域研究與創作人才。</p>
        <div class="line"></div>
        <p class="p14">因應未來產業的發展趨勢，創新科技與當代藝術結合之創作如雨後春筍。清華大學的是國內科學與科技的頂尖學府，對藝術學院發展「科技藝術」具有得天獨厚的優勢。本班師資除來自清華校內藝術學院、電資學院、工學院、生命科學院、人文社會等跨域教師外，我們也將聘進一群來自美國、歐洲與日本跨國與跨域的專業教師。也廣邀在臺灣在科技藝術創作領域最頂尖的業界團隊與藝術家加入我們的教學團隊，讓同學得到專業與多元的指導，並在共享學習、共享創意的環境裡，開創未來的產業，盡情發揮自己的潛能。</p>
      <div class="circle3"></div>
        <p class="p15">GO TO<br>【學士班課程】</p>
    </div>
    

    <div class="footer">
      <img class="photo3" src="https://ipta.nthu.edu.tw/wp-content/themes/hestia/assets/img/slider2.jpg">
      <div class="rectangle4 "></div>
        <p class="p13">院學士班最新訊息</p>
      <p class="p16">最新消息，看這裡!</p>
      <el-carousel :interval="4000" type="card" height="800px" >
       <el-carousel-item v-for="item in newpicture" :key="item">
         <div class="demo-image">
           <div class="block">
             <el-image
                  style="width: 100%; height: 650px;"
                  :src ="item.src"
                  fit="cover"></el-image>
           </div>
         </div>
          <p class="newtitle">{{item.title}}</p>
          <p class="newword">{{item.word}}</p>
       </el-carousel-item>
      </el-carousel>
    </div> 
  </div>
  
  
</template>

<script>
export default {
  name: 'hello',
  data(){
    return{
    newpicture:[
      { src : "https://ipta.nthu.edu.tw/wp-content/uploads/2020/10/banner.png",
        title : "《那顆Ｇ1咻！》國立清華大學藝術學院學士班第一屆系展",
        word : " 「當藝術碰撞科技，會迸出什麼樣的火花呢?」"},
      { src : "https://ipta.nthu.edu.tw/wp-content/uploads/2019/10/board-2303325_1920.jpg",
        title : "2020藝術學院學士班春之清華獎學金",
        word : "【獲獎名單】"},
      { src : "https://ipta.nthu.edu.tw/wp-content/uploads/2020/05/tfho.jpg",
        title:"《科技物件與人類幻象》",
        word:"【講座與工作坊】",},
      { src : "https://ipta.nthu.edu.tw/wp-content/uploads/2020/05/200528.jpg",
        title : "Art and the Brain: A Glimpse of Neuroaesthetics從腦科學看藝術",
        word: "【演講】"},
    ],
    }

},
}
</script>

<style>
.header, .section, .footer {
  position: absolute;
  float: right;
}
  .header {
    position: relative;
    width: 1440px;
    height: 1024px;
    overflow: hidden;
    background: #1F2B39; 
  }
  .logo {
    position: absolute;
    width: 86px;
    height: 87px;
    left: 43px;
    top: 31px;
  }
  .polygon1 {
    position: absolute;
    width: 0px;
    height: 0px;
    left: 975px;
    top: 35px;
    border-right:solid 15px #1F2B39 ;
    border-bottom:solid 15px #ECAA65;
    transform: rotate(315deg);
  }
  .polygon2 {
    position: absolute;
    width: 0px;
    height: 0px;
    left: 1090px;
    top: 35px;
    border-right:solid 15px #1F2B39 ;
    border-bottom:solid 15px #ECAA65;
    transform: rotate(315deg);
  }
  .polygon3 {
    position: absolute;
    width: 0px;
    height: 0px;
    left: 1190px;
    top: 35px;
    border-right:solid 15px #1F2B39 ;
    border-bottom:solid 15px #ECAA65;
    transform: rotate(315deg);
  }
  .polygon4 {
    position: absolute;
    width: 0px;
    height: 0px;
    left: 1318px;
    top: 35px;
    border-right:solid 15px #1F2B39 ;
    border-bottom:solid 15px #ECAA65;
    transform: rotate(315deg);
  }
  .cube1 {
    position: absolute;
    width: 95px;
    height: 65px;
    left: 682px;
    top: 10px;
    background: #1F2B39;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .cube2 {
    position: absolute;
    width: 114px;
    height: 65px;
    left: 789px;
    top: 10px;
    background: #1F2B39;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .cube3 {
    position: absolute;
    width: 84px;
    height: 65px;
    left: 915px;
    top: 10px;
    background: #1F2B39;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .cube4 {
    position: absolute;
    width: 104px;
    height: 65px;
    left: 1011px;
    top: 10px;
    background: #1F2B39;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .cube5 {
    position: absolute;
    width: 84px;
    height: 65px;
    left: 1127px;
    top: 10px;
    background: #1F2B39;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .cube6 {
    position: absolute;
    width: 114px;
    height: 65px;
    left: 1224px;
    top: 10px;
    background: #1F2B39;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .cube7 {
    position: absolute;
    width: 84px;
    height: 65px;
    left: 1349px;
    top: 10px;
    background: #1F2B39;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .photo1 {
    position: absolute;
    width: 2690px;
    height: 878px;
    left: -176px;
    top: 131px;

    mix-blend-mode: soft-light;
    box-shadow: inset 0px 4px 4px rgba(0, 0, 0, 0.25);
  }
  .circle2 {
    position: absolute;
    width: 500px;
    height: 500px;
    left: 469px;
    top: 247px;
    border-radius: 100%;
    background: conic-gradient(from 236.16deg at 50% 50%, #ECAA65 0deg, rgba(236, 170, 101, 0) 360deg);
  }
  .circle1 {
    position: absolute;
    width: 425px;
    height: 425px;
    left: 507px;
    top: 289px;
    border-radius: 100%;
    background: linear-gradient(180deg, #ECAA65 44.71%, rgba(236, 170, 101, 0) 100%);
  }
  .p1 {
   position: absolute;
   width: 350px;
   height: 114px;
   left: 45px;
   top: 90px;
   font-family: Roboto;
   font-style: normal;
   font-weight: normal;
   font-size: 48px;
   line-height: 56px;
   text-align: center;
   letter-spacing: 0.05em;
   color: #1F2B39;
  }
  .p2 {
    position: absolute;
    width: 231px;
    height: 71px;
    left: 110px;
    top: 200px;
    font-family: Roboto;
    font-style: italic;
    font-weight: normal;
    font-size: 48px;
    line-height: 56px;
    text-align: center;
    letter-spacing: 0.41em;
    color: #1F2B39;
  }
  .p3 {
    position: absolute;
    width: 70px;
    height: 33px;
    left: 694px;
    top: 14px;
    font-family: Roboto Condensed;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 23px;
    text-align: center;
    letter-spacing: 0.05em;
    color: #ECAA65;
  }
  .p4 {
    position: absolute;
    width: 117px;
    height: 36px;
    left: 786px;
    top: 14px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    color: #ECAA65;
  }
  .p5 {
    position: absolute;
    width: 98px;
    height: 20px;
    left: 900px;
    top: 14px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    color: #ECAA65;
  }
  .p6 {
    position: absolute;
    width: 84px;
    height: 43px;
    left: 1011px;
    top: 14px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    color: #ECAA65;
  }
  .p7 {
    position: absolute;
    width: 62px;
    height: 35px;
    left: 1134px;
    top: 14px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    color: #ECAA65;
  }
  .p8 {
    position: absolute;
    width: 94px;
    height: 35px;
    left: 1225px;
    top: 14px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    color: #ECAA65;
  }
  .p9 {
    position: absolute;
    width: 48px;
    height: 21px;
    left: 1367px;
    top: 14px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    color: #ECAA65;
  }
  .section {
    position: relative;
    width: 1440px;
    height: 1024px;
    left: 0px;
    top: 0px;
    background: #1F2B39;
    overflow: hidden;
  }
  .p10 {
    position: absolute;
    width: 960px;
    height: 36px;
    left: 235px;
    top: 30px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 25px;
    line-height: 39px;
    text-align: center;
    letter-spacing: 0.07em;
    color: #01060c;
  }
  .p11 {
    position: absolute;
    width: 1009px;
    height: 135px;
    left: 210px;
    top: 240px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 26px;
    line-height: 39px;
    text-align: center;
    letter-spacing: 0.07em;
    color: #01060c;
  }
  .p12 {
    position: absolute;
    width: 490px;
    height: 505px;
    left: 183px;
    top: 463px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 26px;
    line-height: 32px;
    text-align: left;
    letter-spacing: 0.13em;
    color: #212f3f;
  }
  .p14 {
    position: absolute;
    width: 486px;
    height: 538px;
    left: 775px;
    top: 463px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 26px;
    line-height: 32px;
    text-align: left;
    letter-spacing: 0.13em;
    color: #1F2B39;
  }
  .p15 {
    position: absolute;
    width: 161px;
    height: 53px;
    left: 631px;
    top: 950px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 22px;
    text-align: center;
    letter-spacing: 0.13em;
    color: #ECAA65;
  }
  .photo2 {
    position: absolute;
    width: 1975px;
    height: 928px;
    left: -535px;
    top: 45px;
    mix-blend-mode: soft-light;
  }
  .rectangle1 {
    position: absolute;
    width: 1062px;
    height: 204px;
    left: 180px;
    top: 45px;
    background: rgba(249, 246, 243, 0.9);
    filter: blur(4px);
    border-radius: 100px;
  }
  .rectangle2 {
    position: absolute;
    width: 1062px;
    height: 149px;
    left: 180px;
    top: 259px;
    background: rgba(249, 246, 243, 0.9);
    filter: blur(4px);
    border-radius: 100px;
  }
  .rectangle3 {
    position: absolute;
    width: 1182px;
    height: 606px;
    left: 120px;
    top: 432px;
    background: conic-gradient(from -90deg at 105.65% 100%, rgba(249, 246, 243, 0.99) 0deg, rgba(249, 246, 243, 0) 360deg);
    filter: blur(4px);
    border-radius: 41px;
  }
  .line {
    position: absolute;
    width: 500px;
    height: 0px;
    left: 460px;
    top: 700px;
    border: 1px solid #1F2B39;
    transform: rotate(90deg);
  }
  .circle3 {
    position: absolute;
    width: 186px;
    height: 140px;
    left: 620px;
    top: 951px;
    background: #1F2B39;
    border-radius: 60%;
  }
  .footer {
    position: relative;
    width: 1440px;
    height: 1024px;
    background: #1F2B39; 
  }
  .photo3 {
    position: absolute;
    width: 1440px;
    height: 1024px;
    left: 0px;
    top: 0px;
    z-index:1;
  }
  .rectangle4 {
    position: absolute;
    width: 271px;
    height: 45px;
    left: 585px;
    top: 56px;
    background: #EBE8E6;
    filter: blur(4px);
    z-index: 9;
  }
  .p13 {
    position: absolute;
    width: 271px;
    height: 36px;
    left: 590px;
    top: 42px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 26px;
    line-height: 32px;
    letter-spacing: 0.13em;
    color: #1F2B39;
    z-index: 99;
  }
  .p16 {
    position: absolute;
    width: 281px;
    height: 53px;
    left: 585px;
    top: 105px;
    font-family: Quicksand;
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 32px;
    letter-spacing: 0.13em;
    color: #ECAA65;
    z-index: 9999;
  }
  .el-carousel-item{
    font-size: 14px;
    line-height: 200px;
    top: 500px;
    margin: 0;
    Z-index:99999;
  }
  .el-carousel{
    top:200px;
  }
  .newtitle {
    color: #ECAA65;
    font-size:20px; 
  }
  .newword {
    color: #ECAA65;
    font-size:18px;
  }
</style>