<template>
  <div id="app">
    <el-container>
      <el-header height="180px" style="padding: 0;">
        <Header></Header>
      </el-header>
      <el-main style="padding: 0;">
        <Banner></Banner>
        <Theory></Theory>
        <div class="mid-ads">
          <a href="https://saas-shop.jiakaobaodian.com/runtu/cooperate.html" target="_blank"></a>
        </div>
        <RecommendPage>
          </RecommendPage>
          <Page></Page>
          <Glory></Glory>
          <AppList></AppList>
          <Bottom></Bottom>
      </el-main>
    </el-container>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Banner from './components/Banner.vue'
import Theory from './components/Theory.vue'
import Process from './components/Process.vue'
import Glory from './components/Glory.vue'
import AppList from './components/AppList.vue'
import Bottom from './components/Bottom.vue'
import RecommendPage from './components/RecommendPage.vue'
export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Theory,
    Process,
    Glory,
    AppList,
    Bottom,
    RecommendPage
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  min-width: 1200px;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  background-color: #FFFFFF;
}

.el-header {
  background-color: #B3C0D1;
  color: #333;
  text-align: center;
  line-height: 180px;
}

.el-main {
  color: #333;
  text-align: center;
}

.mid-ads {
  width: 100%;
  height: 120px;
  display: block;
  margin: 0 auto;
  background-color: #FFFFFF;
}

a {
  background: url('../public/images/banner-jxb.png') center no-repeat;
  display: block;
  width: 100%;
  height: 100%
}
</style>
