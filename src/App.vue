<template>
  <div id="app">
    哈哈
    <el-steps :active="3" finish-status="success" simple style="margin-top: 20px">
      <el-step title="step 1 、 个人信息"></el-step>
      <el-step title="step 2 、 工作信息"></el-step>
      <el-step title="step 3 、 资产信息"></el-step>
    </el-steps>
    <!--<Container></Container>-->
    <!--<hr>-->
    <!--<el-container>-->
      <!--<el-header>Header</el-header>-->
      <!--<el-main>Main</el-main>-->
      <!--<el-footer>Footer</el-footer>-->
    <!--</el-container>-->
  </div>


</template>

<script>
  // import HelloWorld from './components/HelloWorld'

  import Container from './components/Container'
  export default {
    name: 'App',
    components: {
      Container
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 0px;
  }

  .el-row {
    margin-bottom: 20px;

  &
  :last-child {
    margin-bottom: 0;
  }

  }
  .el-col {
    border-radius: 4px;
  }

  .bg-purple-dark {
    background: #99a9bf;
  }

  .bg-purple {
    background: #d3dce6;
  }

  .bg-purple-light {
    background: #e5e9f2;
  }

  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }

  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }


  .el-header, .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 200px;
  }

  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }

  body > .el-container {
    margin-bottom: 40px;
  }

  .el-container:nth-child(5) .el-aside,
  .el-container:nth-child(6) .el-aside {
    line-height: 260px;
  }

  .el-container:nth-child(7) .el-aside {
    line-height: 320px;
  }
</style>
