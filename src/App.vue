<template>
  <div class="app">
    <el-menu class="app-menu" mode="horizontal" :router="true" :default-active="$route.path">
      <el-menu-item index="/list">事项列表</el-menu-item>
      <el-menu-item index="/add">添加代办事项</el-menu-item>
      <el-menu-item index="/about">关于</el-menu-item>
    </el-menu>

    <router-view class="app-main"></router-view>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';

@Component({})
export default class App extends Vue {}
</script>

<style>
.app {
  max-width: 800px;
  min-height: 100vh;
  margin: 0 auto;
  background-color: #fff;
  overflow: hidden;
}

.app-menu {
  display: flex;
  justify-content: center;
  margin-bottom: 1.6em;
}

.app-main {
  padding: 0 1em;
}
</style>
