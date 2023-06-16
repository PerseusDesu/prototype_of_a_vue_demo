<template>
  <div id="head">
    <div class="line"></div>
    <el-menu :default-active="activeIndex2" class="el-menu-demo" 
    mode="horizontal" @select="handleSelect" 
    background-color="#888888" text-color="#fff" 
    active-text-color="#ffeeff">

        <el-menu-item index="1"><router-link to='/home'>首页</router-link></el-menu-item>
        <el-menu-item index="2"><router-link to='/manager'>后台</router-link></el-menu-item>
        <el-menu-item index="3"><router-link to='/login'>登录</router-link></el-menu-item>
        
    </el-menu>

  </div>
</template>

<script>
  export default {
    name:"TheHead",
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>