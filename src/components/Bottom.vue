<template>
  <div class="container">
    <div class="left">
      <div class="leftItem">
        <span>驾考宝典APP下载</span>
        <p>考驾照 用宝典</p>
      </div>
      <div class="rightItem"></div>
    </div>
    <div class="right">
      <div class="leftItem">
        <span>驾考宝典微信小程序</span>
        <p>无需下载，驾考做题更方便！</p>
      </div>
      <div class="rightItem2"></div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container {
  width: 100%;
  height: 298px;
  background-color: #f5f5f5;
  display: flex;
  justify-content: center;
  align-items: center;
}

.left {
  width: 40%;
  height: 60%;
  border-right: 2px solid #e9e9e9;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.leftItem {
  width: 40%;
  height: 60%;
  font-size: 20px;
  text-align: left;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: start;
}

.leftItem p {
  color: #999;
  font-size: 14px;
}

.rightItem {
  width: 40%;
  height: 60%;
  background-color: green;
  background: url('../../public/images/appDownload.png') center no-repeat;
  background-size: contain;
}

.right {
  width: 40%;
  height: 60%;
  /* background-color: red; */
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.rightItem2 {
  width: 40%;
  height: 60%;
  background-color: green;
  background: url('../../public/images/miniApp.jpg') center no-repeat;
  background-size: contain;
}
</style>