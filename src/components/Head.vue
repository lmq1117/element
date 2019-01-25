<template>
  <el-header>
    <el-menu
      :default-active="activeIndex2"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <el-menu-item index="1">新闻中心</el-menu-item>
      <el-submenu index="2">
        <template slot="title">工作台</template>
        <el-menu-item index="2-1">个人中心</el-menu-item>
        <el-menu-item index="2-2">精彩活动</el-menu-item>
        <el-menu-item index="2-3">热辣派对</el-menu-item>
        <el-submenu index="2-4">
          <template slot="title">常见问题</template>
          <el-menu-item index="2-4-1">如何充值</el-menu-item>
          <el-menu-item index="2-4-2">如何消费</el-menu-item>
          <el-menu-item index="2-4-3">如何退款</el-menu-item>
        </el-submenu>
      </el-submenu>
      <!--<el-menu-item index="3" disabled>消息中心2</el-menu-item>-->
      <el-menu-item index="3">消息中心</el-menu-item>
      <!--<el-menu-item index="4"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item>-->
    </el-menu>
  </el-header>
</template>

<script>
  export default {
    name: 'Head',
    data() {
      return {
        msg: 'HEAD title',
        activeIndex: '1',
        activeIndex2: '1'
      }
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
