<template>
    <div>
  <template>
  <el-tabs v-model="activeName" style="margin:0 5% 0 5%">
    <el-tab-pane label="全部" name="first">
      <div style="height:auto;width:100%;display:inline-flex;border-bottom-color:#fff" v-for="item in newlist[0]" :key="item.id">
      <div class="NewsPicture">
      <img :src=item.imgurl style="  width: auto; height: auto;  max-width: 100%;  max-height: 100%;">
      </div>
      <div class="NewsMain">
      <h2 class="NewsTitle">
      <a href="">{{item.title}}</a>
      </h2>
      <div style="width:732px;height:124px;margin-bottom:80px">{{item.bodys}}</div>
      </div>
      </div>
    </el-tab-pane>
    <el-tab-pane label="评测" name="second">
      <div style="height:auto;width:100%;display:inline-flex;border-bottom-color:#fff" v-for="item in newlist[1]" :key="item.id">
      <div class="NewsPicture">
      <img :src=item.imgurl style="  width: auto; height: auto;  max-width: 100%;  max-height: 100%;">
      </div>
      <div class="NewsMain">
      <h2 class="NewsTitle">
      <a href="">{{item.title}}</a>
      </h2>
      <div style="width:732px;height:124px;margin-bottom:80px">{{item.bodys}}</div>
      </div>
      </div>
    </el-tab-pane>
    <el-tab-pane label="新闻" name="third">
             <div style="height:auto;width:100%;display:inline-flex;border-bottom-color:#fff" v-for="item in newlist[2]" :key="item.id">
      <div class="NewsPicture">
      <img :src=item.imgurl style="  width: auto; height: auto;  max-width: 100%;  max-height: 100%;">
      </div>
      <div class="NewsMain">
      <h2 class="NewsTitle">
      <a href="">{{item.title}}</a>
      </h2>
      <div style="width:732px;height:64px;margin-bottom:80px" class="test">{{item.bodys}}</div>
      </div>
      </div>
    </el-tab-pane>
  </el-tabs>
</template>
    </div>
</template>
<script>
export default {
  data () {
    return {
      activeName: 'second',
      newlist: [
        [
          {id: 1, title: '雾霾天生存攻略：出门N95在家用yobbom!', bodys: '“关于雾霾君的前世今生，此处省略无穷无尽字数，毕竟小编不是自带科普Buff的《芈月传》剧组，为推剧将春秋战国史给捣鼓了个底朝天。言归正传，既然雾霾君降临时喊破喉咙也没有用，还是想想怎么尽可能安全、舒心的扛过雾霾天才是硬道理。接下来，请欣赏小编为大家精心整理的雾霾天小攻略，如有抄袭纯属雷同没有版权欢迎转载。不过话说回来，对付雾霾这样无孔不入的灾祸，小心驶得万年船这样的传统逻辑还是有一定的道理。譬如能见…', ctime: '2017-05-16', imgurl: '../../../../../static/img/an3.png'},
          {id: 2, title: '把家庭影院装进音响——音磅YOBBOM90 智能音响评测', bodys: '“说到音响，大家的第一反应大致是一个方方正正的盒子用于播放声音。可是你听说过能看电影、电视剧的音响吗？你又听说过可以唱卡拉OK、玩游戏的音响吗？音磅就是这样一款主打音乐，同时又集合了影视剧播放、听音乐、KTV点歌、游戏等功能的智能影院音响。下面就请跟随高清范评测君来看看这款音磅YOBBOM90智能影视音响的实际表现吧。外观：打开外包装，这就是今天的主角啦音磅YOBBOM90，可以看到音磅本体还是非常…', ctime: '2017-11-5', imgurl: '../../../../../static/img/an4.png'},
          {id: 3, title: '音磅60=小米音响+电视主机，这款智能音响电视游戏K歌无所不能！', bodys: '“自从小米电视3代推出分体电视以来，很久没有创新的电视行业刮起了一阵旋风，分体电视这一脱离传统电视的模式引起了广泛的关注，那么将显示屏、主机和音响三者分离后，真的会带来一场全新的视听革命吗？这让我想起了极米的无屏电视，实际上不管有屏无屏，基本的诉求都可以满足，那么这场较量的根本在于能否让用户获得更加个性化的体验。近期面市的音磅60一体智能音响[Office1]事实上就是这样一款产品，像极了小米电视的...', imgurl: '../../../../../static/img/an2.png'},
          {id: 4, title: '音磅s-90智能音响评测 不止于声 智能畅享', bodys: '引言“音响”可以说是我们生活中再熟悉不过的东西，而随着人们对音响“挑剔”程度的不断增加，智能音响应运而生。什么是智能音响？就是在保有优质声音的前提下，加入了智能硬件，使其更加人性化、多元化、智能化，可是说是传统音响的进阶产物。其不但可以实现WIFI、蓝牙、NFC等技术，还可以与电脑、手机等无线设备，真正的实现智能一体化。在当前快餐式生活节奏下，人们追…', WBtnVaule: '', ctime: '2017-05-16', imgurl: '../../../../../static/img/an1.png'}
        ],
        [
          {id: 1, title: '音磅S60荣获2018“金耳朵选择”认证', bodys: '音磅S60荣获2018“金耳朵选择”认证10.11日，全球最大的采购电子展——GlobalSource2018盛大开幕。在展会中，中国电子音响协会举办2018大众音频产品“金耳朵选择”颁奖典礼。音磅一体智能音响S60,继获得国际IF设计奖、工信部最具创新应用产品奖后，凭借影院般体验的音质音效和整体科技创新，再次荣获了&ldqu…', WBtnVaule: '', ctime: '2017-05-16', imgurl: '../../../../../static/img/an5.png'},
          {id: 2, title: '高性价比畅想无线乐趣 音磅idol蓝牙耳机', bodys: '随着国内消费升级，在耳机电子消费类市场，出现了越来越多样式的耳机产品，互联网音响品牌音磅(YOBBOM)也发布了一款新品——音磅真无线蓝牙耳机idol，以超高的性价比重新定义全民无线耳机，为无线耳机市场注入了新的活力。音磅idol耳机完美解决了用户对耳机线缆、续航、音质等方面的需求痛点，带来更好的使用体验和更高品质的音乐享受；外观采用了黑白两种经典配色，阴阳协调，极具美感。', WBtnVaule: '', ctime: '2017-11-5', imgurl: '../../../../../static/img/an6.png'},
          {id: 3, title: '269元 真无线真自由 音磅真无线蓝牙耳机idol开箱图赏', bodys: '随着越来越多的手机产品砍掉3.5mm耳机孔，无线蓝牙耳机的发展迎来绝佳契机。获得过多个企业产品创新奖的音磅其声（YOBBOM）公司最近推出了一款真无线蓝牙耳机idol。这款耳机非常的轻盈小巧，单边耳机比1元硬币还轻，优化的人体工程学设计，适合人耳的侧入耳角度机身设计，贴合耳廓，长时间佩戴舒适无压痛感，在运动中和出街时，大动作摇摆也不会脱落，非常稳固。国内首款采用蓝牙5.0芯片，它传输速度是普通蓝牙', WBtnVaule: '', ctime: '2017-11-5', imgurl: '../../../../../static/img/an7.png'},
          {id: 4, title: '音磅亮相SSHT 打造“家庭娱乐生活”新样本', bodys: '9月3日至5日，音磅（Yobbom）应邀参加上海国际智能家居展览会，本届SSHT汇聚了紫光、海信、旷视、阿尔卡特、小狗机器人等公司机构，集中展示一年来智能家居领域的最新发展成果。音磅创立于2014年，由多位音响互联网、人工智能等领域的博士及专家团队共同组建，以智能声学硬件为主打产品，自深耕音频行业以来，取得了非凡的成绩，此次展会上，音磅携带了一体智能狂想90系列、狂想60系列等产品，向行业展示了当…', ctime: '2017-05-16', imgurl: '../../../../../static/img/an8.png'}
        ],
        [
          {id: 1, title: '音磅亮相SSHT 打造“家庭娱乐生活”新样本', bodys: '9月3日至5日，音磅（Yobbom）应邀参加上海国际智能家居展览会，本届SSHT汇聚了紫光、海信、旷视、阿尔卡特、小狗机器人等公司机构，集中展示一年来智能家居领域的最新发展成果。音磅创立于2014年，由多位音响互联网、人工智能等领域的博士及专家团队共同组建，以智能声学硬件为主打产品，自深耕音频行业以来，取得了非凡的成绩，此次展会上，音磅携带了一体智能狂想90系列、狂想60系列等产品，向行业展示了当…', ctime: '2017-05-16', imgurl: '../../../../../static/img/an8.png'},
          {id: 2, title: '高性价比畅想无线乐趣 音磅idol蓝牙耳机', bodys: '随着国内消费升级，在耳机电子消费类市场，出现了越来越多样式的耳机产品，互联网音响品牌音磅(YOBBOM)也发布了一款新品——音磅真无线蓝牙耳机idol，以超高的性价比重新定义全民无线耳机，为无线耳机市场注入了新的活力。音磅idol耳机完美解决了用户对耳机线缆、续航、音质等方面的需求痛点，带来更好的使用体验和更高品质的音乐享受；外观采用了黑白两种经典配色，阴阳协调，极具美感。', WBtnVaule: '', ctime: '2017-11-5', imgurl: '../../../../../static/img/an6.png'},
          {id: 3, title: '音磅60=小米音响+电视主机，这款智能音响电视游戏K歌无所不能！', bodys: '“自从小米电视3代推出分体电视以来，很久没有创新的电视行业刮起了一阵旋风，分体电视这一脱离传统电视的模式引起了广泛的关注，那么将显示屏、主机和音响三者分离后，真的会带来一场全新的视听革命吗？这让我想起了极米的无屏电视，实际上不管有屏无屏，基本的诉求都可以满足，那么这场较量的根本在于能否让用户获得更加个性化的体验。近期面市的音磅60一体智能音响[Office1]事实上就是这样一款产品，像极了小米电视的...', imgurl: '../../../../../static/img/an2.png'},
          {id: 4, title: '音磅s-90智能音响评测 不止于声 智能畅享', bodys: '引言“音响”可以说是我们生活中再熟悉不过的东西，而随着人们对音响“挑剔”程度的不断增加，智能音响应运而生。什么是智能音响？就是在保有优质声音的前提下，加入了智能硬件，使其更加人性化、多元化、智能化，可是说是传统音响的进阶产物。其不但可以实现WIFI、蓝牙、NFC等技术，还可以与电脑、手机等无线设备，真正的实现智能一体化。在当前快餐式生活节奏下，人们追…', WBtnVaule: '', ctime: '2017-05-16', imgurl: '../../../../../static/img/an1.png'}
        ]
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
  .NewsMain
    @media screen and (min-width:1200px){
        float:right
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
    @media screen and (max-width:1199px){
        float:right
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
    @media screen and (max-width:992px){
        float:right
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
    @media screen and (max-width:768px){
        float:right
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
    @media screen and (max-width:520px){
        float:right
        width:66%
        height:320px
        margin: 0 3% 2.8% 0
    }
  .NewsPicture
    @media screen and (min-width:1200px){
        width:300px
        height: 200px
        cursor: pointer
        transition: all 0.6s
        float:left
        width:28%
        height:320px
        margin: 0 3% 3% 2.7%
    }
    @media screen and (max-width:1199px){
        width:300px
        height: 200px
        cursor: pointer
        transition: all 0.6s
        float:left
        width:28%
        height:320px
        margin: 0 3% 3% 2.7%
    }
    @media screen and (max-width:992px){
        width:300px
        height: 200px
        cursor: pointer
        transition: all 0.6s
        float:left
        width:28%
        height:320px
        margin: 0 3% 3% 2.7%
    }
    @media screen and (max-width:768px){
        width:300px
        height: 200px
        cursor: pointer
        transition: all 0.6s
        float:left
        width:28%
        height:320px
        margin: 0 3% 3% 2.7%
    }
    @media screen and (max-width:520px){
        width:300px
        height: 200px
        cursor: pointer
        transition: all 0.6s
        float:left
        width:28%
        height:320px
        margin: 0 3% 3% 2.7%
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
    border:1px solid lightblue;height:28px;width:80px;float:right;color:#007ce3;padding:3px;margin:3px;text-align:center
  .NewsPicture:hover
    transform:scale(0.9)
    overflow:hidden
  .test
    text-overflow ellopsis
    height 64px
    </style>
