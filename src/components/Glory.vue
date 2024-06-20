<template>
  <div class="container">
    <div class="content">
      <div class="title-container">
        <p class="title">宝典荣誉</p>
        <div class="title2">强大的驾考功能，优秀的用户体验，我们的愿景是学车无忧，轻松拿本</div>
      </div>
      <div class="function">

      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container {
  margin-top: -100px;
  /* background-color: #FFFFFF; */
  width: 100%;
  height: 510px;
  display: flex;
  justify-content: center;
  align-items: center;
  /* background-color: #000; */
}

.content {
  width: 80%;
  height: 75%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}

.title-container {
  width: 100%;
  height: 1%;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.title {
  position: relative;
  font-size: 30px;
  text-align: center;
}

.title::before,
.title::after {
  content: '';
  position: absolute;
  top: 50%;
  width: 100%;
  border-bottom: 2px dotted #E9E9E9;
  transform: translateY(-50%);
}

.title::before {
  left: -110%;
  margin-right: 10px;
}

.title::after {
  right: -110%;
  margin-left: 10px;
}

.title2 {
  font-size: 16px;
  color: #666;
}

.function {
  width: 100%;
  height: 85%;
  background-color: aqua;
  background: url('../../public/images/Glory.png') center no-repeat;
}
</style>
