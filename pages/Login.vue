<template>
  <div class="flex flex-row ...">
      <div class="left-img">
        <img src="/assets/GH.jpg" alt="">
      </div>
      <div class="right-text">

        <img src="../assets/login/avatar.svg" style="margin: auto; width: 100px;height: 100px" alt="">
        <h1>Pure-admin</h1>
        <div class="login-auto">
          <el-form-item>
          <el-input type="" v-model="username" placeholder="请输入用户名" show-password clearable></el-input>
        </el-form-item>
        <el-form-item>
          <el-input type="password" v-model="userpassword" placeholder="请输入密码" show-password clearable></el-input>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" style="width: 100%;" @click="login()">登录</el-button>
        </el-form-item>
          <el-divider>
            第三方登录
          </el-divider>
        <div class=" grid grid-cols-3 gap-4 content-center ..." style="display: flex;justify-content: space-between;">
        <el-form-item>
          <el-button type="primary" style="width: 100px;background: white">手机登录</el-button>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" style="width: 100px;background: white">二维码登录</el-button>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" style="width: 100px;background: white">注册</el-button>
        </el-form-item>
        </div>
        </div>
      </div>
  </div>
</template>

<style scoped lang="less">
.img1{
  position: absolute;
  top: 20%;
}
.left-img{
  background-color: #999999;
  width: 50%;
  height: 700px;
  padding: 90px 20px 100px;
  img{
    width: 100%;
    border-radius: 10px;
  }
}
.right-text{
  //background-color: blueviolet;
  width: 50%;
  height: 150%;
  h1{
    font-size: 50px;
    color: #999999;
    margin-top: 100px;
    text-align: center;
  }
  .login-auto{
    width: 70%;
    // background-color: blue;
    margin: auto;
  }
}
</style>

<script lang="ts" setup>
import {defineComponent} from 'vue'

defineComponent({
  name: "Login"
})
definePageMeta({
  layout: false,
})
const username = ref('')
const userpassword = ref('')
const router = useRouter()
const login = () => {
  if(username.value === 'admin' || userpassword.value === '0'){
    alert('登录成功')
    router.push('/')
  }

  // router.push('/Editor')
}
</script>