<template>
  <div id="app">
    <el-container>
      <el-header>
        <MyHeader />
      </el-header>
      <el-container class="forum-container">
        <router-view />
      </el-container>
    </el-container>
  </div>
</template>

<script>
import MyHeader from "./views/header";

export default {
  name: "App",
  components: {
    MyHeader
  }
};
</script>

<style lang="less" scoped>
.el-header {
  padding: 0;
  background: #fff;
  box-shadow: 0 1px 3px rgba(26, 26, 26, 0.1);
  background-clip: content-box;
  overflow: hidden;
  position: fixed;
  left: 0;
  right: 0;
  z-index: 10;
}
.el-container {
  background: #f6f6f6;
}

.forum-container {
  display: flex;
  width: 1000px;
  margin: 10px auto;
  margin-top: 70px;
}
</style>
