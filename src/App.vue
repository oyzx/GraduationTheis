<template>
  <div id="app">
    <nav class="navbar navbar-default" role="navigation">
      <div class="container-fluid">
        <div class="navbar-header">
          <button type="button" class="navbar-toggle collapsed" @click="navbarCollapsed = !navbarCollapsed">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          <a class="navbar-brand" href="#">10号先生</a>
        </div>
        <div class="navbar-collapse" :class="navbarCollapsed ? 'collapsed' : 'collapse'">
          <ul class="nav navbar-nav">
            <li class="active"><router-link to="/basis">基本信息</router-link></li>
            <li><router-link to="/supply">供应链信息</router-link></li>
            <li><router-link to="/order">订单管理</router-link></li>
            <li><router-link to="/data">数据统计</router-link></li>
          </ul>
        </div>
      </div>
    </nav>
    <div class="container-fluid">
      <div class="row">
        <div class="col-md-7">
          <router-view></router-view>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import home from './component/home.vue'
export default {
  data () {
    return {
      navbarCollapsed:false
    }
  },
  components: { home }
}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>