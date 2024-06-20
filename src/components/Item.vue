<template>
  <a class="item" :style="{ backgroundImage: 'url(' + imageUrl + ')' }" @mouseover="hovering = true" @mouseleave="hovering = false" :href=itemObj.link target="_blank">
    <span style="font-size: 24px; color: #333;">{{ itemObj.title }}</span>
    <p style="font-size: 14px; color: #666;">{{ itemObj.title2 }}</p>
  </a>
</template>

<script>
export default {
  props: {
    itemObj: {
      type: Object,
      required: true
    }
  },
  data() {
    return {
      hovering: false
    };
  },
  computed: {
    imageUrl() {
      return this.hovering ? this.itemObj.hoverUrl : this.itemObj.imageUrl;
    }
  }
}
</script>

<style scoped>
a {
  text-decoration: none;
}

.item {
  width: 15%;
  height: 75%;
  background-repeat: no-repeat;
  background-position: top center;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
  cursor: pointer;
}

.item:hover {
  color: #37B5F8;
  /* Change color on hover */
  background-image: none;
  /* Remove background image on hover */
}
</style>
