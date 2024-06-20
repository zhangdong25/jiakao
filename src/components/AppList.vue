<template>
  <div class="container">
    <div class="div1">
      <div class="content">
        <div class="title">教练宝典APP</div>
        <div class="imgContainer">
          <div class="imgShow"></div>
          <div class="imgHover"></div>
        </div>
      </div>
    </div>
    <div class="div2">
      <div class="content2">
        <div class="title">驾考宝典APP</div>
        <div class="imgContainer">
          <div class="imgShow2"></div>
          <div class="imgHover2"></div>
        </div>
      </div>
    </div>
    <div class="div3">
      <div class="content3">
        <div class="title">买车宝典APP</div>
        <div class="imgContainer">
          <div class="imgShow3"></div>
          <div class="imgHover3"></div>
        </div>
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
  width: 100%;
  height: 80vh;
  background-color: #f5f5f5;
  overflow: hidden;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: space-between;
}

.div1,
.div3 {
  width: 300px;
  height: 100%;
  position: relative;
}

.div2 {
  width: 400px;
  height: 100%;
  position: relative;
}

.div3 {
  width: 290px;
  height: 100%;
  position: relative;
}

.content {
  position: absolute;
  width: 100%;
  height: 80%;
  animation: moveDown 1s forwards;
}

.content:hover {
  animation: moveUp 1s forwards;
}

.content2 {
  position: absolute;
  width: 100%;
  height: 90%;
  animation: moveDown2 1s forwards;
}

.content2:hover {
  animation: moveUp2 1s forwards;
}

.content3 {
  position: absolute;
  width: 100%;
  height: 70%;
  top: 30%;
  animation: moveDown3 1s forwards;
}

.content3:hover {
  animation: moveUp3 1s forwards;
}

@keyframes moveUp {
  from {
    top: 30%;
  }

  to {
    top: 20%;
  }
}

@keyframes moveDown {
  from {
    top: 20%;
  }

  to {
    top: 30%;
  }
}

@keyframes moveUp2 {
  from {
    top: 16%;
  }

  to {
    top: 10%;
  }
}

@keyframes moveDown2 {
  from {
    top: 10%;
  }

  to {
    top: 16%;
  }
}

@keyframes moveUp3 {
  from {
    top: 40%;
  }

  to {
    top: 30%;
  }
}

@keyframes moveDown3 {
  from {
    top: 30%;
  }

  to {
    top: 40%;
  }
}

.imgContainer {
  position: relative;
  width: 100%;
  height: 92%;
}

.title {
  width: 100%;
  height: 8%;
  text-align: center;
  font-size: 20px;
}

.imgShow,
.imgHover,
.imgShow3,
.imgHover3 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-size: contain;
  background-position: center;
  background-repeat: no-repeat;
  transition: opacity 0.5s;
}

.imgShow2 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-size: contain;
  background-position: bottom;
  background-repeat: no-repeat;
  transition: opacity 0.5s;
}

.imgHover2 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-size: 45%;
  background-position: center;
  background-repeat: no-repeat;
  transition: opacity 0.5s;
}

.imgShow {
  background-image: url('../../public/images/app1.png');
  z-index: 1;
}

.imgHover {
  background-image: url('../../public/images/app1Code.png');
  z-index: 2;
  opacity: 0;
}

.imgShow2 {
  background-image: url('../../public/images/app2.png');
  z-index: 1;
}

.imgHover2 {
  background-image: url('../../public/images/app2Code.png');
  z-index: 2;
  opacity: 0;
}

.imgShow3 {
  background-image: url('../../public/images/app3.png');
  z-index: 1;
}

.imgHover3 {
  background-image: url('../../public/images/app3Code.png');
  z-index: 2;
  opacity: 0;
}

.content:hover .imgHover {
  opacity: 1;
}

.content:hover .imgShow {
  opacity: 1;
}

.content2:hover .imgHover2 {
  opacity: 1;
}

.content2:hover .imgShow2 {
  opacity: 1;
}

.content3:hover .imgHover3 {
  opacity: 1;
}

.content3:hover .imgShow3 {
  opacity: 1;
}
</style>