<template>
  <div id="app">
    <div class="header">
      <img class="logo" src="https://ipta.nthu.edu.tw/wp-content/uploads/2019/02/cropped-NTHU-logo.png">
      <div class="cube1"></div>
      <div class="cube2"></div>
      <div class="cube3"></div>
      <div class="cube4"></div>
      <div class="cube5"></div>
      <div class="cube6"></div>
      <div class="cube7"></div>
      <img class="photo1" src="https://ipta.nthu.edu.tw/wp-content/uploads/2017/10/BG.jpg">
      <div class="circle2"></div>
        <div class="circle1">
            <div class="word1">
              國立清華大學
            </div>
        </div>
    </div>
    <div class="section">
      <img class="photo2" src="https://ipta.nthu.edu.tw/wp-content/uploads/2017/10/BG.jpg">
      <div class="rectangle1"></div>
      <div class="rectangle2"></div>
      <div class="rectangle3"></div>
    </div>
    <div class="footer">
      <img class="photo3" src="https://ipta.nthu.edu.tw/wp-content/themes/hestia/assets/img/slider2.jpg">
      <div class="rectangle4"></div>
      <el-carousel :interval="4000" type="card" height="300px">
       <el-carousel-item v-for="item in newpicture" :key="item">
         <div class="demo-image">
           <div class="block">
             <el-image
                  style="width: 100%; height: 200px"
                  :src ="item.src"
                  fit="cover"></el-image>
           </div>
         </div>
          <p class="newstitle">{{item.title}}</p>
          <p class="newsword">{{item.word}}</p>
       </el-carousel-item>
      </el-carousel>
    </div> 
  </div>
  
  
</template>
<script>
export default {
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
</script>

<style>
.header, .section, .footer {
  position: absolute;
  float:left;
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
  .word1 {
    position: absolute;
    width: 301px;
    height: 156px;
    left: 570px;
    top: 429px;
    font-family: Roboto Condensed ;
    font-style: normal;
    font-weight: normal;
    font-size: 48px;
    line-height: 56px;
    text-align: center;
    letter-spacing: 0.05em;
    color: #1F2B39;
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
  .footer {
    position: relative;
    width: 1440px;
    height: 1024px;
    overflow: hidden;
    background: #1F2B39; 
  }
  .photo3 {
    position: absolute;
    width: 1440px;
    height: 1024px;
    left: 0px;
    top: 0px;
  }
  .rectangle4 {
    position: absolute;
    width: 271px;
    height: 45px;
    left: 585px;
    top: 56px;
    background: #EBE8E6;
    filter: blur(4px);
  }
   .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }

</style>