<template>
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" active-text-color="#F9FCFE">
    <el-menu-item index="1" class="el-menu-item-demo">首页</el-menu-item>
    <el-submenu index="2" class="el-menu-demo">
      <template slot="title">模拟考试</template>
      <el-menu-item index="2-1" class="el-menu-item-hover">科目一</el-menu-item>
      <el-menu-item index="2-2" class="el-menu-item-hover">科目二</el-menu-item>
      <el-menu-item index="2-3" class="el-menu-item-hover">科目三</el-menu-item>
      <el-menu-item index="2-4" class="el-menu-item-hover">科目四</el-menu-item>
    </el-submenu>
    <el-submenu index="3" class="el-menu-demo">
      <template slot="title">找驾校</template>
      <el-menu-item index="3-1" class="el-menu-item-hover">找驾校</el-menu-item>
      <el-menu-item index="3-2" class="el-menu-item-hover">找教练</el-menu-item>
      <el-menu-item index="3-3" class="el-menu-item-hover">找陪练</el-menu-item>
    </el-submenu>
    <el-menu-item index="4" class="el-menu-item-demo">驾考圈</el-menu-item>
    <el-menu-item index="5" class="el-menu-item-demo">交通标志</el-menu-item>
    <el-menu-item index="6" class="el-menu-item-demo">软件下载</el-menu-item>
    <el-menu-item index="7" class="el-menu-item-demo">驾考宝典企业版</el-menu-item>
    <el-menu-item index="8" class="el-menu-item-demo">智慧驾校</el-menu-item>
    <el-submenu index="9" class="el-menu-demo">
      <template slot="title">买新车</template>
      <el-menu-item index="9-1" class="el-menu-item-hover">买车网</el-menu-item>
      <el-menu-item index="9-2" class="el-menu-item-hover">平行之家</el-menu-item>
    </el-submenu>
    <el-menu-item index="10" class="el-menu-item-demo">二手车</el-menu-item>
  </el-menu>
</template>

<script>
export default {
  data() {
    return {
      activeIndex: '1'
    }
  },
};
</script>

<style scoped>
.el-menu-demo {
  display: flex;
  justify-content: center;
  background-color: #37B5F8;
  color: #F9FCFE;
}


.el-menu-item-demo {
  font-size: 16px !important;
  min-width: 108px;
  min-height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #F9FCFE;
}

/* 改变选中菜单项的背景颜色 */
.el-menu-item-demo.is-active {
  background-color: #258FC7 !important;
}

/* 使用 ::v-deep 穿透作用域，修改子菜单标题的样式 */
::v-deep .el-submenu .el-submenu__title {
  color: #F9FCFE !important;
}

::v-deep .el-submenu .el-submenu__title:hover {
  color: #F9FCFE !important;
  background-color: #54C0F9 !important;
}

/* 改变鼠标悬停时的背景颜色 */
.el-menu-item-demo:hover {
  min-width: 108px;
  min-height: 50px;
  background-color: #54C0F9 !important;
  color: #F9FCFE !important;
}

.el-menu-item-hover {
  display: flex;
  align-items: center;
  justify-content: center;
  color: #F9FCFE;
  font-size: 16px !important;
}

.el-menu-item-hover:hover {
  color: #258FC7 !important;
}
</style>
