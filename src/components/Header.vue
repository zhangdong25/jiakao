<template>
  <div class="container">
    <div class="logoContainer">
      <a class="logo" href="https://dalian.jiakaobaodian.com/"></a>
    </div>
    <div class="searchContainer">
      <el-input type="text" v-model="input" placeholder="请输入关键字" id="input" style="width: 200px;"></el-input>
      <el-button type="info" id="btn">搜索</el-button>
    </div>
    <MyNav class="nav"></MyNav>
  </div>
</template>

<script>
import MyNav from './MyNav.vue'
export default {
  data() {
    return {
      input: ''
    }
  },
  components: {
    MyNav
  },

}
</script>

<style scoped>
.container {
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 100%;
  background-color: #fff;
  position: relative;
}

.logoContainer {
  width: 270px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.logo {
  width: 270px;
  height: 50px;
  background: url('../../public/images/logo.png') left center no-repeat;
  vertical-align: middle;
}

.searchContainer {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 500px;
  height: 42px;
}

#input {
  height: 42px;
  border: none;
  border-radius: 0px;
  font-size: 14px;
}

#btn {
  text-align: center;
  height: 42px;
  border-radius: 0px;
  background-color: #F0F0F0;
  color: #333;
  font-size: 14px;
  border: none;
}
.nav {
  position: absolute;
  bottom: 0;
  width: 100%;
}
</style>