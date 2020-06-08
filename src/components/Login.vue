<template>
  <div class="login_container">
    <div class="login_window">
      <div class="head_portrait">
        <img src="./../assets/logo.jpg" alt />
      </div>
      <!-- 登录区 -->
      <el-form label-width="0px" class="login_form">
        <!-- 用户名 -->
        <el-form-item>
          <el-input prefix-icon="el-icon-user-solid"></el-input>
        </el-form-item>
        <!-- 密码 -->
        <el-form-item>
          <el-input prefix-icon="el-icon-lock"></el-input>
        </el-form-item>
        <!-- 按钮区域 -->
        <el-form-item class="btns">
           <el-button type="primary">登录</el-button>
           <el-button type="info">重置</el-button>
        </el-form-item>
      </el-form>
    </div>
  </div>
</template>
<script>
export default {}
</script>

<style lang="scss" scoped>
.login_container {
  background: #ffaa00;
  height: 100%;
}

.login_window {
  width: 450px;
  height: 300px;
  background: #ffffff;
  border-radius: 3px;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  .head_portrait {
    height: 130px;
    width: 130px;
    border: 1px solid #eee;
    border-radius: 50%;
    padding: 10px;
    box-shadow: 0 0 10px #ddd;
    position: absolute;
    left: 50%;
    transform: translate(-50%, -50%);
    background: #ffffff;
    img {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      background: #eee;
    }
  }
}
.login_form{
    position: absolute;
    bottom: 0;
    width: 100%;
    padding: 0 20px;
    box-sizing: border-box;
}
.btns{
    display: flex;
    justify-content: flex-end;
}
</style>
