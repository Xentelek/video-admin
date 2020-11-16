<template>
  <div class="container">
    <div class="site-title">
      <span>Colors</span>
    </div>
    <div class="menu-bar" ref="menuRef">
      <a href="/dashboard" class="menus">
        <div class="item" :class="{ select: isActive }">
          <i class="iconfont icon-NMStubiao-"></i>
        </div>
        <span :class="{ 'item-color': isActive }">Dashboard</span>
      </a>
      <a href="" class="menus">
        <div class="item">
          <i class="iconfont icon-LC_icon_message_line"></i>
        </div>
        <span class="menu-color">Messages</span>
      </a>
      <a href="" class="menus">
        <div class="item">
          <i class="iconfont icon-chat-smile-line"></i>
        </div>
        <span>Chats</span>
      </a>
      <a href="" class="menus">
        <div class="item">
          <i class="iconfont icon-Profile"></i>
        </div>
        <span>Profile</span>
      </a>
      <a href="" class="menus">
        <div class="item">
          <i class="iconfont icon-upload"></i>
        </div>
        <span>Upload</span>
      </a>
      <a href="" class="menus">
        <div class="item">
          <i class="iconfont icon-Settingscontroloptions"></i>
        </div>
        <span>Settings</span>
      </a>
      <a href="" class="menus">
        <div class="item">
          <i class="iconfont icon-Profile"></i>
        </div>
        <span>User</span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: true
    };
  },
  mounted() {
    console.log(this.$refs.menuRef);
  }
};
</script>

<style scoped lang="scss">
.container {
  height: 100%;
  width: 200px;
  border-right: 1px solid #ccc;
  display: flex;
  flex-direction: column;
  .site-title {
    height: 100px;
    line-height: 100px;
    margin: 0 auto;
    font-size: 20px;
    font-family: Arial, Helvetica, sans-serif;
    color: pink;
    font-weight: 600;
  }
  .menu-bar {
    flex: 1;
    border-top: 1px solid #ccc;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    .menus {
      text-decoration: none;
      //   border: 1px solid #ccc;
      flex: 1;
      display: flex;
      flex-direction: row;
      //   justify-content: space-evenly;
      align-items: center;
      .item {
        width: 40%;
        height: 50%;
        padding-right: 10px;
        // border: 1px solid tomato;
        display: flex;
        justify-content: flex-end;
        align-items: center;
      }
      span {
        padding-left: 5px;
      }
      .select {
        background-color: #f4eae1;
        border-top-right-radius: 20px;
        border-bottom-right-radius: 20px;
      }
      .item-color {
        color: tomato;
      }
    }
  }
}
</style>
