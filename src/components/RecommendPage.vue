<template>
  <div class="container">
    <div class="content">
      <div class="title-container">
        <p class="title">学车流程</p>
        <div class="title2">驾考宝典整合学车全流程，驾考宝典为用户提供全方位学车服务</div>
      </div>
      <div class="function">
        <Item v-for="(item, index) in items" :key="index" :item-obj="item"></Item>
      </div>
    </div>
  </div>
</template>

<script>
import Item from './Item.vue';

export default {
  components: {
    Item,
  },
  data() {
    return {
      items: [
        { imageUrl: require('/public/images/Process1.png'), hoverUrl: require('/public/images/Process1_hover.png'), title: '找驾校', title2: '口碑好的驾校', link: 'https://www.jiakaobaodian.com/dalian/school/' },
        { imageUrl: require('/public/images/Process2.png'), hoverUrl: require('/public/images/Process2_hover.png'), title: '科目一', title2: '驾驶员理论考试', link: 'https://www.jiakaobaodian.com/mnks/kemu1/car-dalian.html' },
        { imageUrl: require('/public/images/Process3.png'), hoverUrl: require('/public/images/Process3_hover.png'), title: '科目二', title2: '场地驾驶技能考试科目', link: 'https://www.jiakaobaodian.com/mnks/kemu2/car-dalian.html' },
        { imageUrl: require('/public/images/Process4.png'), hoverUrl: require('/public/images/Process4_hover.png'), title: '科目三', title2: '机动车驾驶人道路考试', link: 'https://www.jiakaobaodian.com/mnks/kemu3/car-dalian.html' },
        { imageUrl: require('/public/images/Process5.png'), hoverUrl: require('/public/images/Process5_hover.png'), title: '科目四', title2: '安全文明驾驶常识考试', link: 'https://www.jiakaobaodian.com/mnks/kemu4/car-dalian.html' },
        { imageUrl: require('/public/images/Process6.png'), hoverUrl: require('/public/images/Process6_hover.png'), title: '拿本', title2: '开心拿本, 安全驾驶', link: '#' }
      ]
    };
  }
}
</script>

<style scoped>
.container {
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
}
</style>
