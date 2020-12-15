
<template>
  <div>
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
              @click="aaa">点我去看主页</button>
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
      activeNames: ['1']
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
</style>


