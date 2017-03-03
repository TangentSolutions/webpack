<template>
  <div id="app">
    <el-row>
      <el-col :span="24">
      <app-header></app-header>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="8">
        <!-- should be: <side-nav :items='..' ></side-nav> -->
        <side-nav></side-nav>
      </el-col>
      <el-col :span="16">
        <img src="./assets/logo.png">
        <router-view></router-view>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import AppHeader from './components/pages/AppHeader'
import SideNav from './components/pages/SideNav'

export default {
  name: 'app',
  components: { AppHeader, SideNav }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
