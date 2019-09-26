<template>
  <div id="main">
  <el-tabs v-model="activeName" style="margin: 0 5% 0 5%">
    <el-tab-pane label="安心保障" name="first">
    <div v-for="item in newlist[0]" :key="item.id" class="service1">
        <img :src=item.imgurl />
        <h1 class="title">{{item.title}}</h1>
        <h6 style="font-size:2rem;">{{item.subtitle}}</h6>
    </div>
    </el-tab-pane>
    <el-tab-pane label="使用说明" name="second">
      <div v-for="item in newlist[1]" :key="item.id" class="img">
        <img :src=item.imgurl alt="" style="width: auto; height: auto;  max-width: 200%;  max-height: 200%;margin:0px;margin-left:-400px">
      </div>
    </el-tab-pane>
    <el-tab-pane label="应用下载" name="third">
      <div class="app">
        <img src="../../../../../static/img/yapp_03.jpg" alt="" style="float:right">
        <div class="app2">
          <h1 style="margin:8px;font-size:3rem;">音磅APP</h1>
          <span style="font-size:20px;">操作控制，用户交流，手机投屏，</span>
          <div style="font-size:20px;">音磅所有功能可以用APP控制，更方便，更快速</div>
        </div>
      </div>
    </el-tab-pane>
    <el-tab-pane label="售后" name="four">
      <div>
        <div>
          <ul>
            <li v-for="item in newlist[2]" :key="item.title" class="slafe">{{item.title}}</li>
          </ul>
        </div>
        <div></div>
      </div>
    </el-tab-pane>
  </el-tabs>
    </div>
</template>
<script>
export default {
  data () {
    return {
      activeName: 'first',
      newlist: [
        [
          {id: 1, title: '七天无理由退货', subtitle: '从购买音磅产品起7天内，凭购买凭证，可联系客服进行无理由退货服务。', WBtnVaule: '', ctime: '2017-05-16', imgurl: '../../../../../static/img/1.png'},
          {id: 2, title: '1年放心使用', subtitle: '从购买音磅产品起1年内，享受整机质保服务。', ctime: '2017-11-5', imgurl: '../../../../../static/img/2.png'},
          {id: 3, title: '3年主要部件保修', subtitle: '音磅产品主要部件均提供3年质保服务，请联系客服详细了解。', WBtnVaule: '', ctime: '2017-11-5', imgurl: '../../../../../static/img/3.png'},
          {id: 4, title: '技术专家上门服务', subtitle: '部分地区可提供专家上门服务。', WBtnVaule: '', ctime: '2017-05-16', imgurl: '../../../../../static/img/4.png'}
        ],
        [
          {id: 1, imgurl: '../../../../../static/img/p1.jpg'},
          {id: 2, imgurl: '../../../../../static/img/p2.jpg'},
          {id: 3, imgurl: '../../../../../static/img/p3.jpg'},
          {id: 4, imgurl: '../../../../../static/img/p4.jpg'},
          {id: 5, imgurl: '../../../../../static/img/p5.jpg'},
          {id: 6, imgurl: '../../../../../static/img/p6.jpg'},
          {id: 7, imgurl: '../../../../../static/img/p7.jpg'}
        ],
        [
          {id: 1, title: '服务与支持', bodys: '“关于雾霾君的前世今生，此处省略无穷无尽字数，毕竟小编不是自带科普Buff的《芈月传》剧组，为推剧将春秋战国史给捣鼓了个底朝天。言归正传，既然雾霾君降临时喊破喉咙也没有用，还是想想怎么尽可能安全、舒心的扛过雾霾天才是硬道理。接下来，请欣赏小编为大家精心整理的雾霾天小攻略，如有抄袭纯属雷同没有版权欢迎转载。不过话说回来，对付雾霾这样无孔不入的灾祸，小心驶得万年船这样的传统逻辑还是有一定的道理。譬如能见…', WBtnVaule: '', ctime: '2017-05-16', imgurl: '../../static/img/1.png'},
          {id: 2, title: '售后政策', bodys: '“音响”可以说是我们生活中再熟悉不过的东西，而随着人们对音响“挑剔”程度的不断增加，智能音响应运而生。什么是智能音响？就是在保有优质声音的前提下，加入了智能硬件，使其更加人性化、多元化、智能化，可是说是传统音响的进阶产物。其不但可以实现WIFI、蓝牙、NFC等技术，还可以与电脑、手机等无线设备，真正的实现智能一体化。', WBtnVaule: '', ctime: '2017-11-5', imgurl: '../../static/img/2.jpg'},
          {id: 3, title: '保修服务', bodys: '“音响”可以说是我们生活中再熟悉不过的东西，而随着人们对音响“挑剔”程度的不断增加，智能音响应运而生。什么是智能音响？就是在保有优质声音的前提下，加入了智能硬件，使其更加人性化、多元化、智能化，可是说是传统音响的进阶产物。其不但可以实现WIFI、蓝牙、NFC等技术，还可以与电脑、手机等无线设备，真正的实现智能一体化。', WBtnVaule: '', ctime: '2017-11-5', imgurl: '../../static/img/4.jpg'}
        ]
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
  .service1
    margin:0px
    @media screen and (min-width:1200px){
        width:100%
        margin-bottom:120px
        text-align:center
    }
    @media screen and (max-width:1199px){
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
    @media screen and (max-width:992px){
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
    @media screen and (max-width:768px){
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
    @media screen and (max-width:520px){
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
  .NewsTitle
    font-weight: bold
    text-align:left
  a:hover
    color: #007ce3
  a
    text-decoration:none
    color:#000
  .NewsBtn
    border:1px solid lightblue;height:28px;width:80px;float:right;color:#007ce3
  .NewsPicture:hover
    transform:scale(0.4)
  .title
    font-size:3rem;margin-top:-10px;margin-bottom:40px;text-align:center
  .img
    margin-top:-25px
  #main >.el-tabs__header
    padding: 0;
    position: relative;
    margin: 0px;
  .app
    url(../../../../../static/img/yapp_03.jpg)right -30px center no-repeat;
  .app2
    position:absolute;
    margin-left:40px
    margin-top:400px
  .slafe
    width:200px;height:60px;border:1px solide #fff;font-size:20px;padding:15px 40px 15px 40px
    </style>
