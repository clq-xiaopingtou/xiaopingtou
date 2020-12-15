
<template>
  <div>
    <!-- 头部 -->
    <div class="jianli1">
      <div class="jianli2">
        <h1>简历展示</h1>
      </div>
    </div>

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

    <div id="but">
      <button class="but1"
              @click="aaa">点我去看项目</button>
      <button class="but2"
              @click="bbb">点我去看随机</button>
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
      width1: 0 + '%',
      width2: 0 + '%',
      width3: 0 + '%',
      width4: 0 + '%',
      width5: 0 + '%',
      width6: 0 + '%',
      width7: 0 + '%',

    };
  },
  //方法 函数写这里
  methods: {
    aaa () {
      this.$router.push({ path: '/demo' })
    },
    bbb () {
      this.$router.push({ path: '/login' })
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
    window.addEventListener('scroll', this.scrollToTop)
    window.addEventListener(
      "scroll",
      (e) => {
        // console.log("我进入了scroll监听  ");
        let top = document.documentElement.scrollTop;
        if (top > 200) {
          // 改变width
          this.width1 = 85 + '%'
          this.width2 = 76 + '%'
          this.width3 = 65 + '%'
          this.width4 = 80 + '%'
          this.width5 = 60 + '%'
          this.width6 = 50 + '%'
          this.width7 = 78 + '%'
          // console.log(this.$refs)
          // this.$refs.html1.style.width = 200 +'px'
          // this.$refs.html1.style.width = 95 +'%'
        } else {
          // console.log('111222333');

          // 控制顶部动画
          // clearInterval(timerr)
        }
        // console.log(top);
        // 这个是判断顶部的
        if (top > 200) {
          this.sticky = true
        } else {
          this.sticky = false
        }
      },
      true
    );
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





<style lang="scss">
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
  // background-color: skyblue;
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
  // background-color: blueviolet;
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


