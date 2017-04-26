<template>
  <div id="app">
    <nav class="navbar navbar-default" role="navigation">
      <div class="container-fluid">
        <div class="navbar-header">
          <button type="button" class="navbar-toggle collapsed">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          <a class="navbar-brand" href="#">10号先生</a>
        </div>
        <div class="navbar-collapse">
          <ul class="nav navbar-nav">
            <li class="active"><a router-link to="/disi">基本信息</a></li>
            <li><a router-link to="/diwu">供应链信息</a></li>
            <li><a href="#">订单管理</a></li>
            <li><a href="#">数据统计</a></li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>