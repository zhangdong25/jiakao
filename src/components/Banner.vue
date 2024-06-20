<template>
  <div class="container">
    <el-carousel interval="4000" trigger="click" arrow="never" style="height: 100%; width: 100%;">
      <el-carousel-item v-for="(item, index) in images" :key="item">
        <el-image :src="item" fit="cover" style="width: 100%; height: 100%;" @click="handleClick(index)">{{ item }}</el-image>
      </el-carousel-item>
    </el-carousel>
    <div class="banner-menu">
      <div class="banner-menu-title">
        <div class="title-text">学车流程</div>
      </div>
      <div class="banner-menu-content">
        <div class="content">
          <a target="_blank" href="https://www.jiakaobaodian.com/mnks/kemu1/car-dalian.html" class="link">
            科目一
            <p style="margin: -10px 0 0 0; font-size: 14px; color: #666;">2024新题库</p>
          </a>
        </div>
        <div class="content">
          <a target="_blank" href="https://www.jiakaobaodian.com/mnks/kemu2/car-dalian.html" class="link2">
            科目二
            <p style="margin: -10px 0 0 0; font-size: 14px; color: #666;">精选视频，详解考点</p>
          </a>
        </div>
        <div class="content">
          <a target="_blank" href="https://www.jiakaobaodian.com/mnks/kemu3/car-dalian.html" class="link3">
            科目三
            <p style="margin: -10px 0 0 0; font-size: 14px; color: #666;">全方位讲解，攻克难点</p>
          </a>
        </div>
        <div class="content">
          <a target="_blank" href="https://www.jiakaobaodian.com/mnks/kemu4/car-dalian.html" class="link4">
            科目四
            <p style="margin: -10px 0 0 0; font-size: 14px; color: #666;">2024新题库</p>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        'images/home_banner_download.png',
        'images/home_banner_new1.jpeg',
        'images/home_banner_jiaolian.jpg',
        'images/home_banner_jiaxiaobang.png',
      ],
      adsUrl: [
        'https://www.jiakaobaodian.com/download/',
        'https://www.mucang.cn/company/honor/',
        'https://www.mucang.cn/jiaolianbaodian/?from=jxrz-topbanner',
        'https://saas-shop.jiakaobaodian.com/runtu/cooperate.html',
      ],
    }
  },
  methods: {
    handleClick(item) {
      console.log(item)
      window.open(this.adsUrl[item], '_blank');
    }
  }
}
</script>

<style lang="less" scoped>
.container {
  width: 100%;
  height: 380px;
  position: relative;
}

.banner-menu {
  width: 280px;
  height: 340px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: rgba(255, 255, 255, .9);
  position: absolute;
  left: 160px;
  top: 20px;
  z-index: 10;
}

.banner-menu-title {
  width: 250px;
  height: 20%;
}

.title-text {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  text-align: center;
  font-size: 20px;
  border-bottom: 1px dotted #ddd;
}

.banner-menu-content {
  width: 250px;
  height: 80%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.content {
  width: 100%;
  height: 25%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: start;
}

a {
  text-decoration: none;
}

.link {
  display: block;
  color: #37B5F8;
  padding: 10px 0 0 50px;
  line-height: 30px;
  margin: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: start;
  height: 100%;
  background: url('../../public/images/1.png') left center no-repeat;
  background-size: 40px;
  font-size: 16px;
  text-align: left;
}

.link2 {
  display: block;
  color: #37B5F8;
  padding: 10px 0 0 50px;
  line-height: 30px;
  margin: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: start;
  height: 100%;
  background: url('../../public/images/2.png') left center no-repeat;
  background-size: 40px;
  font-size: 16px;
  text-align: left;
}

.link3 {
  display: block;
  color: #37B5F8;
  padding: 10px 0 0 50px;
  line-height: 30px;
  margin: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: start;
  height: 100%;
  background: url('../../public/images/3.png') left center no-repeat;
  background-size: 40px;
  font-size: 16px;
  text-align: left;
}

.link4 {
  display: block;
  color: #37B5F8;
  padding: 10px 0 0 50px;
  line-height: 30px;
  margin: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: start;
  height: 100%;
  background: url('../../public/images/4.png') left center no-repeat;
  background-size: 40px;
  font-size: 16px;
  text-align: left;
}

/deep/ .el-carousel {
  width: 100%;
  height: 100%;
}

/deep/ .el-carousel__container {
  width: 100%;
  height: 100%;
}

/deep/ .el-carousel__container {
  width: 100%;
  height: 100%;
}

/deep/.el-carousel__indicators--horizontal {
  width: 70px;
  display: flex;
  text-align: center;

  .el-carousel__indicator--horizontal button {
    width: 8px;
    height: 8px;
    background: #95C3CC;
    border-radius: 50%;
    opacity: 0.5;
  }

  .el-carousel__indicator--horizontal.is-active button {
    width: 8px;
    height: 8px;
    background: #007AFF;
    opacity: 0.5;
    border-radius: 50%;
  }
}
</style>