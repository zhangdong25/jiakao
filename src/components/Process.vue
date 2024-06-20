<template>
  <div class="container">
    <div class="content">
      <div class="title-container">
        <p class="title">学车流程</p>
        <div class="title2">驾考宝典整合学车全流程，驾考宝典为用户提供全方位学车服务</div>
      </div>
      <div class="function">
        <a class="item">
          <span style="font-size: 24px;">找驾校</span>
          <p style="font-size: 16px; color: #666;">口碑好的驾校</p>
        </a>
        <a class="item">
          <span style="font-size: 24px;">找驾校</span>
          <p style="font-size: 16px; color: #666;">口碑好的驾校</p>
        </a>
        <a class="item">
          <span style="font-size: 24px;">找驾校</span>
          <p style="font-size: 16px; color: #666;">口碑好的驾校</p>
        </a>
        <a class="item">
          <span style="font-size: 24px;">找驾校</span>
          <p style="font-size: 16px; color: #666;">口碑好的驾校</p>
        </a>
        <a class="item">
          <span style="font-size: 24px;">找驾校</span>
          <p style="font-size: 16px; color: #666;">口碑好的驾校</p>
        </a>
        <a class="item">
          <span style="font-size: 24px;">找驾校</span>
          <p style="font-size: 16px; color: #666;">口碑好的驾校</p>
        </a>
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
  width: 100%;
  height: 510px;
  display: flex;
  justify-content: center;
  align-items: center;
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
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  align-items: center;
  /* background-color: aqua; */
}

.item {
  width: 15%;
  height: 75%;
  background-color: red;
  background: url('../../public/images/Process1.png') top no-repeat;
  /* background-color: aqua; */
  display: flex;
  flex-direction: column;
  justify-content: end;
  align-items: center;
  cursor: pointer;
}

.item:hover {
  background: url('../../public/images/Process1_hover.png') top no-repeat;
  color: #37B5F8;
}
</style>
