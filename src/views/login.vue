
<template>
  <div>

    <!-- 介绍 -->
    <div v-show="a">
      <!-- 展示 -->
      <div class="zhanshi">
        <div class="zhanshi1">
          <!-- 姓名 -->
          <!-- 左 -->
          <div class="nei1">
            <div class="span1">
              <svg class="icon"
                   aria-hidden="true">
                <use xlink:href="#icon-icon-test"></use>
              </svg>
              <h3 class="span1-h3">姓名：陈龙强</h3>

            </div>
            <div class="span1">
              <svg class="icon"
                   aria-hidden="true">
                <use xlink:href="#icon-dianhua"></use>
              </svg>
              <h3 class="span1-h3">电话：15933377804</h3>

            </div>
            <div class="span1">
              <svg class="icon"
                   aria-hidden="true">
                <use xlink:href="#icon-youxiang"></use>
              </svg>
              <h3 class="span1-h3">邮箱：xiaopingtouclq@163.com</h3>

            </div>
            <div class="span1">
              <svg class="icon"
                   aria-hidden="true">
                <use xlink:href="#icon-weixin"></use>
              </svg>
              <h3 class="span1-h3">微信：c2404831604</h3>

            </div>
            <div class="span1">
              <svg class="icon"
                   aria-hidden="true">
                <use xlink:href="#icon-QQ"></use>
              </svg>
              <h3 class="span1-h3">QQ：2404831604</h3>

            </div>

          </div>
          <!-- 右 -->
          <div class="nei2">

            <div class="nei21">
              <h2>技能掌握</h2>
            </div>

            <p> 1. 熟练使用原生javascript以及jquery库，熟悉es6新特性，对css/javascript性能优化，解决多浏览器兼容问题有一定经验。</p>

            <p>2. 精通html/javascript/css/ajax等前端相关技术，理解web开发原理，熟悉常用前端框架，如vue，react。</p>

            <p> 3. 熟练使用前端框架Vue+vuex+elememtui+vant进行组件化开发，对React有所涉及。</p>
            <p> 4. 熟练使用jquery，element-ui，lin-ui，vant，Bootstrap等工具。</p>
            <p>5. 熟练使用非关系型数据库mysql以及关系型mongodb数据库。</p>
            <p> 6. 熟练使用git，进行多人协作开发。</p>
            <p> 7. 会使用ps做一些简单的裁剪切图。</p>
            <p>8. 对nodejs有一定了解，能使用express模板开启一个服务器，连接数据库编写接口并解决跨域等问题。</p>
            <p> 9. 关注微信小程序，对小程序开发有一定了解。</p>
          </div>

        </div>
      </div>
    </div>

    <!-- 技能条 -->
    <div v-show="b">
      <!-- 技能展示 -->
      <section data-x
               id="siteSkills"
               class="skills">
        <h2 class="jineng">技能</h2>

        <li>
          <h3>
            HTML 5 &amp; CSS 3
          </h3>
          <div class="progressBar">
            <div ref="html1"
                 class="progress"
                 :style="{width:width1}"></div>
          </div>
        </li>
        <li>
          <h3>
            JavaScript
          </h3>
          <div class="progressBar">
            <div class="progress"
                 :style="{width:width2}"
                 style="transition-delay:1s"></div>
          </div>
        </li>
        <li>
          <h3>
            jQuery
          </h3>
          <div class="progressBar">
            <div class="progress"
                 :style="{width:width3}"
                 style="transition-delay:2s"></div>
          </div>
        </li>
        <li>
          <h3>
            Vue.js
          </h3>
          <div class="progressBar">
            <div class="progress"
                 :style="{width:width4}"
                 style="transition-delay:3s"></div>>
          </div>
        </li>
        <li>
          <h3>
            React.js
          </h3>
          <div class="progressBar">
            <div class="progress"
                 :style="{width:width5}"
                 style="transition-delay:4s"></div>
          </div>
        </li>
        <li>
          <h3>
            Node.js
          </h3>
          <div class="progressBar">
            <div class="progress"
                 :style="{width:width6}"
                 style="transition-delay:5s"></div>
          </div>
        </li>
        <li>
          <h3>
            小程序
          </h3>
          <div class="progressBar">
            <div class="progress"
                 :style="{width:width7}"
                 style="transition-delay:6s"></div>
          </div>
        </li>

      </section>
    </div>

    <!-- 项目 -->
    <div v-show="c">
      <el-collapse v-model="activeNames"
                   @change="handleChange">

        <el-collapse-item title="项目名称：YOODOO"
                          name="1">
          <div>项目简介：
            YOODOO是一款为消费者打造的购票平台，拥有独立的会员体系，支持在线选座，优惠购票。 </div>
          <div>项目周期：6个月</div>
          <div>项目要点：
            1：使用Vue全家桶作为技术栈，
            2：使用axios实现前后端的数据交互，
            3：使用vant进行页面布局，
            4：使用Vuex进行公共数据管理；使用eventBus进行页面状态管理，
            5：对代码和性能进行优化，</div>
          <div>项目职责：
            负责组件页面的搭建，完成首页、商城页和活动页面布局以及各功能的实现，使用Git进行多人协作开发。</div>
        </el-collapse-item>

        <el-collapse-item title="项目名称：厚e贷"
                          name="2">
          <div>项目描述：
            厚e贷是一款提供借贷服务的软件，操作安全并且无隐患。</div>
          <div>项目周期：4个月</div>
          <div>项目要点：
            1：使用rem对页面进行适配，
            2：使用Vue框架进行页面组件化开发，
            3：使用vant-ui组件实现页面效果。</div>
          <div>项目职责：
            负责底层架构的搭建，完成首页、产品页的数据渲染和登录注册功能的实现，使用eventBus对页面状态进行管理，使用Git进行多人协作开发。</div>
        </el-collapse-item>

        <el-collapse-item title="项目名称：嗨省商购"
                          name="3">
          <div>项目描述：
            嗨省电商是一家互联网的商贸公司，是一款为商家服务，让更多的商家卖货更简单的平台。</div>
          <div>项目周期：6个月</div>
          <div>项目技术要点：
            使用vue框架进行组件化开发，对用户的登录状态进行判断，商家推广功能的实现。</div>
          <div>项目职责：
            根据要求完成页面的开发，页面交互，特效功能的实现，
            和后端人员一起完成前后端的交互，数据的渲染。</div>
        </el-collapse-item>

        <el-collapse-item title="项目名称：红绿蓝后台"
                          name="4">
          <div>项目描述：
            本次项目是基于Vue开发的学生以及会员后台管理系统，可以对学生和会员的基本信息，课程信息以及会员信息进行管理和查看，让学生和会员后台信息统一管理操作变得更加快捷。</div>
          <div>项目周期：4个月</div>
          <div>项目要点：
            1：使用Vue框架作为项目的基础框架，
            2：判断路由的权限和侧边栏的权限来实现不同权限用户所访问的模块的不同。</div>
          <div>项目职责：
            负责整个后台管理系统的页面布局及效果实现，负责与后端人员进行接口联调，会员管理页面和权限列表页面功能的实现，后期项目需求的更新迭代和bug修复。</div>
        </el-collapse-item>
      </el-collapse>

      <div id="but">
        <button class="but1"
                @click="aaa">点我去主页</button>
        <button class="but2"
                @click="bbb">点我去看项目</button>
      </div>
    </div>

    <div id="but">
      <button class="but1"
              @click="aaa">点我去看主页</button>
      <button class="but2"
              @click="bbb">点我去看项目</button>
    </div>
  </div>
</template>



<script>
export default {
  //组件名字
  name: "moban",
  //接收父组件给的东西 type是接收什么东西  default 默认值
  props: {
    list: {
      type: Array,
      default () {
        return [];
      }
    },
    color: {
      type: String,
      default: '#000'
    }
  },
  //组件注册
  components: {},
  // vue数据集中管理
  data () {
    return {
      value: "1",
      activeNames: ['1'],
      width1: 0 + '%',
      width2: 0 + '%',
      width3: 0 + '%',
      width4: 0 + '%',
      width5: 0 + '%',
      width6: 0 + '%',
      width7: 0 + '%',
      b: false,
      c: false,
      a: true,
      bianhua: 0
    };
  },
  //方法 函数写这里
  methods: {
    handleChange (val) {
      console.log(val);
    },
    aaa () {
      this.$router.push({ path: '/' })
    },
    bbb () {
      this.$router.push({ path: '/demo' })

    },
    ccc () {
      this.bianhua++
      console.log(this.bianhua);
      if (this.bianhua === 10) {
        this.b = true
        this.a = false
        this.c = false
      }
      if (this.bianhua === 20) {
        this.c = true
        this.a = false
        this.b = false
      }
      if (this.bianhua === 30) {
        this.bianhua = 0
        this.a = true
        this.b = false
        this.c = false

      }
    }








  },
  //计算属性
  computed: {},
  //侦听器
  watch: {},
  //过滤器
  filters: {
    toUpcase (value) {
      return value ? value.toUpperCase() : ''
    },
  },
  //以下是生命周期 
  //组件创建之前  new操作符桥梁函数return 之前
  beforeCreate () {

  },
  //组件创建之后
  created () {

  },
  //页面渲染之前
  beforeMount () {

  },
  //页面渲染之后
  mounted () {

    let time = setInterval(() => {
      this.ccc()
    }, 1000)




    if (this.bianhua = 20) {
      this.width1 = 85 + '%'
      this.width2 = 80 + '%'
      this.width3 = 80 + '%'
      this.width4 = 75 + '%'
      this.width5 = 70 + '%'
      this.width6 = 70 + '%'
      this.width7 = 78 + '%'
    }









  },
  //页面销毁之前
  beforeDestroy () {

  },
  //页面销毁之后
  destroyed () {

  },
  //页面视图数据更新之前
  beforeUpdate () {

  },
  //页面视图数据更新之后
  updated () {

  },
  //组件路由守卫enter
  beforeRouteEnter (to, from, next) {
    next(vm => { });
    // 注意，在路由进入之前，组件实例还未渲染，所以无法获取this实例，只能通过vm来访问组件实例
  },
  //组件路由守卫update更新
  beforeRouteUpdate (to, from, next) {
    // 同一页面，刷新不同数据时调用，
    next();
  },
  //组件路由守卫离开
  beforeRouteLeave (to, from, next) {
    // 离开当前路由页面时调用
    next();
  }
};
</script>





<style  lang="scss">
* {
  margin: 0;
  padding: 0;
}
body,
html {
  background: url("https://ftp.bmp.ovh/imgs/2020/12/3c45f3fde24e2ff0.jpg");
}
// tou
.jianli1 {
  width: 100%;
  text-align: center;
}
// 展示
.zhanshi {
  margin-top: 50px;
  // text-align: center;
  width: 100%;
  height: 400px;
}
.zhanshi1 {
  width: 800px;
  height: 400px;
  margin: auto;
  background-color: skyblue;
}
.nei1 {
  width: 400px;
  height: 400px;
  float: left;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}
.nei2 {
  float: right;
  width: 400px;
  height: 400px;
  background-color: blueviolet;
}
// 左
.icon {
  width: 40px;
  height: 30px;
  line-height: 40px;
}
.span1 {
  width: 100%;
  height: 40px;
  display: flex;
  align-items: center;
}
.span1-h3 {
  margin-top: 0;
  display: inline-block;
}

// 右
.nei21 {
  width: 100%;
  text-align: center;
}
.nei2 p {
  margin-top: 3px;
}
// 技能条

section.skills,
section.portfolio {
  max-width: 940px;
  margin-left: auto;
  margin-right: auto;
  margin-top: 60px;
  // box-shadow: 2px 2px 2px 2px;
  // opacity: 0.7;
}
section.skills > h2,
section.portfolio > h2 {
  text-align: center;
  color: #3d4451;
  font-size: 34px;
  line-height: 1.2;
  font-weight: 600;
}
section.skills h3 {
  font-size: 14px;
  line-height: 1.1;
  padding-right: 40px;
}
section.skills > ol {
  background: white;
  box-shadow: 3px 3px 3px 3px;
  padding: 42px 50px 10px;
  margin-top: 30px;
}
section.skills > ol > li {
  float: left;
  width: 48%;
  box-sizing: border-box;
}
section.skills > ol > li:nth-child(even) {
  float: right;
}
section.skills .progressBar {
  height: 5px;
  background: skyblue;
  border-radius: 2px;
  margin: 4px 0 40px;
  overflow: hidden;
}
section.skills .progressBar > .progress {
  height: 100%;
  // background: blue;
  // background: -webkit-gradient(left, 0% 0%, 0% 100%, from(Black), to(blue));
  background: -webkit-linear-gradient(left, blue, black);
  width: 70%;
  border-radius: 2px;
  transform: translateX(0);
  transition: all 1s;
}
section.skills.offset .progress {
  transform: translateX(-100%);
}

section.portfolio {
  text-align: center;
  margin-bottom: 100px;
}
section.portfolio > nav {
  text-align: center;
}
section.portfolio > nav > ol {
  margin: 0 auto;
  display: inline-block;
  vertical-align: top;
}
section.portfolio > nav > ol > li {
  float: left;
  margin-left: 40px;
  cursor: pointer;
}
section.portfolio > nav > ol > li:first-child {
  margin-left: 0;
}
section.portfolio > nav {
  display: inline-block;
  vertical-align: top;
  margin-top: 32px;
}
section.portfolio > nav .bar {
  height: 5px;
  background: white;
  margin-top: 5px;
  margin-bottom: 28px;
  border-radius: 2px;
}
section.portfolio > nav .bar-inner {
  height: 100%;
  background: black;
  border-radius: 2px;
  transition: all 0.3s;
}
section.portfolio > nav .bar.state-1 .bar-inner {
  margin-left: 0;
  width: 50px;
}
section.portfolio > nav .bar.state-2 .bar-inner {
  margin-left: 65px;
  width: 50px;
}
section.portfolio > nav .bar.state-3 .bar-inner {
  margin-left: 140px;
  width: 96px;
}
section.portfolio .works {
  position: relative;
}
section.portfolio .works > .big,
section.portfolio .works > .small {
  position: absolute;
}
#tiao {
  border-radius: 10px;
  background-color: white;
  box-shadow: 2px 2px 2px 2px;
}
#but {
  width: 100%;
  margin-top: 80px;
}
.but1 {
  width: 1000px;
  margin-left: calc(50% - 500px);
  height: 50px;
  background: white;
  transition: all 0.5s;
}
.but1:hover {
  background-color: black;
  color: white;
}
.but2:hover {
  background-color: black;
  color: white;
}
.but2 {
  transition: all 0.5s;
  background: white;
  margin-top: 20px;
  height: 50px;
  width: 1000px;
  margin-left: calc(50% - 500px);
}
li {
  list-style: none;
}
</style>


