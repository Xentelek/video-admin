<template>
  <div class="home">
    <xen-slide></xen-slide>
    <div class="main">
      <xen-header class="header"></xen-header>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import XenSlide from "@/components/XenSlide.vue";
import XenHeader from "@/components/XenHeader.vue";
export default {
  name: "Home",
  components: {
    XenSlide,
    XenHeader
  }
};
</script>
<style lang="scss" scoped>
.home {
  // padding : 40px ;
  // box-sizing: border-box;
  height: 92%;
  width: 95%;
  border-radius: 20px;
  background-color: #fff;
  display: flex;
  .main {
    border: 1px solid red;
    flex: 1;
    .header {
      height: 100px;
      border: 1px solid blueviolet;
    }
  }
}
</style>
