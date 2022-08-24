<template>
  <div class="header">
    <img :src="image" alt="" />
  </div>
</template>

<script>
import image from "@/assets/logo.png";
export default {
  data() {
    return {
      image: image,
    };
  },
};
</script>

<style lang="scss" scoped>
.header {
  margin: 0 auto;
  display: flex;
  margin-bottom: 20px;
  justify-content: center;
  //   border: 2px solid red;
  border-bottom: 2px solid gainsboro;
  padding: 0;

  img {
    width: 90px;
    box-sizing: border-box;
  }
}
</style>