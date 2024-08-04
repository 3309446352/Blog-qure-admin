<template>
  <div class="Collapse"> 

      <div class="icon">
        
      </div>
    <div>
<!--      <el-radio-group v-model="isCollapse" style="margin-bottom: 20px">-->
<!--        <el-radio-button :value="false">expand</el-radio-button>-->
<!--        <el-radio-button :value="true">collapse</el-radio-button>-->
<!--      </el-radio-group>-->
      <img src="../assets/login/avatar.svg" class="icon-avatar" alt="avatar"/>
      <div class="icon-name">PureAdmin</div>
      <el-menu default-active="2" class="el-menu-vertical-demo" :collapse="isCollapse" @open="handleOpen"
        @close="handleClose">
        <el-menu-item index="1">

            <el-icon><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" viewBox="0 0 1024 1024" style="outline: none;" class="iconify iconify--ep"><path fill="currentColor" d="M512 128L128 447.936V896h255.936V640H640v256h255.936V447.936z"></path></svg></el-icon>
            <template #title><router-link to="/"><span>页面</span></router-link></template>

        </el-menu-item>

        <el-sub-menu index="2">
          <template #title>
            <el-icon>
              <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" viewBox="0 0 24 24" style="outline: none;" class="iconify iconify--ri"><path fill="currentColor" d="M12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10s-4.477 10-10 10m0-2a8 8 0 1 0 0-16a8 8 0 0 0 0 16M11 7h2v2h-2zm0 4h2v6h-2z"></path></svg>
            </el-icon>
            <span>异常页面</span>
          </template>
          <el-menu-item-group>
            <el-menu-item index="1-1"><router-link to="/Error/404">404</router-link></el-menu-item>
            <el-menu-item index="1-2"><router-link to="/Error/403">403</router-link></el-menu-item>
            <el-menu-item index="1-2"><router-link to="/Error/500">500</router-link></el-menu-item>
          </el-menu-item-group>
        </el-sub-menu>

        <el-sub-menu index="3">
          <template #title>
            <el-icon>
              <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" viewBox="0 0 1024 1024" class="iconify iconify--ep" style="outline: none;"><path fill="currentColor" d="M513.28 448a64 64 0 1 1 76.544 49.728A96 96 0 0 0 768 448h64a160 160 0 0 1-320 0zm-126.976-29.696a256 256 0 1 0 43.52-180.48A256 256 0 0 1 832 448h-64a192 192 0 0 0-381.696-29.696m105.664 249.472L285.696 874.048a96 96 0 0 1-135.68-135.744l206.208-206.272a320 320 0 1 1 135.744 135.744m-54.464-36.032a322 322 0 0 1-45.248-45.248L195.2 783.552a32 32 0 1 0 45.248 45.248l197.056-197.12z"></path></svg>
            </el-icon>
            <span>权限页面</span>
          </template>
          <el-menu-item-group>
            <el-menu-item index="2-1">导航1</el-menu-item>
            <el-menu-item index="2-2">导航2</el-menu-item>
          </el-menu-item-group>
        </el-sub-menu>

        <el-sub-menu index="4">
          <template #title>
            <el-icon>
              <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" viewBox="0 0 1024 1024" class="iconify iconify--ep" style="outline: none;"><path fill="currentColor" d="M513.28 448a64 64 0 1 1 76.544 49.728A96 96 0 0 0 768 448h64a160 160 0 0 1-320 0zm-126.976-29.696a256 256 0 1 0 43.52-180.48A256 256 0 0 1 832 448h-64a192 192 0 0 0-381.696-29.696m105.664 249.472L285.696 874.048a96 96 0 0 1-135.68-135.744l206.208-206.272a320 320 0 1 1 135.744 135.744m-54.464-36.032a322 322 0 0 1-45.248-45.248L195.2 783.552a32 32 0 1 0 45.248 45.248l197.056-197.12z"></path></svg>
            </el-icon>
            <span>图片页面</span>
          </template>
          <el-menu-item-group>
            <el-menu-item index="3-1"><router-link to="Images">图片</router-link></el-menu-item>
            <el-menu-item index="3-2"><router-link to="Timeline">时间戳</router-link></el-menu-item>
            <el-menu-item index="3-2"><router-link to="Card">卡片</router-link></el-menu-item>
          </el-menu-item-group>
        </el-sub-menu>

        <el-menu-item index="5">

          <el-icon><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" viewBox="0 0 1024 1024" style="outline: none;" class="iconify iconify--ep"><path fill="currentColor" d="M832 512a32 32 0 1 1 64 0v352a32 32 0 0 1-32 32H160a32 32 0 0 1-32-32V160a32 32 0 0 1 32-32h352a32 32 0 0 1 0 64H192v640h640z"></path><path fill="currentColor" d="m469.952 554.24l52.8-7.552L847.104 222.4a32 32 0 1 0-45.248-45.248L477.44 501.44l-7.552 52.8zm422.4-422.4a96 96 0 0 1 0 135.808l-331.84 331.84a32 32 0 0 1-18.112 9.088L436.8 623.68a32 32 0 0 1-36.224-36.224l15.104-105.6a32 32 0 0 1 9.024-18.112l331.904-331.84a96 96 0 0 1 135.744 0z"></path></svg></el-icon>
          <template #title><router-link to="/Editor"><span>编辑器</span></router-link></template>

        </el-menu-item>

        <el-menu-item index="6">
          <el-icon style="width: 60px;height: 70px"><img src="../assets/GH.jpg" alt=""></el-icon>
          <span><router-link to="User">用户界面</router-link></span>
        </el-menu-item>
      </el-menu>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import router from "#app/plugins/router";
const isCollapse = ref(false)
const handleOpen = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
const handleClose = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}

</script>

<style lang="less">
.Collapse {
  background-color: #fdfdfd;
}

.el-menu-vertical-demo:not(.el-menu--collapse) {
  width: 200px;
  min-height: 400px;
}

.icon-name{
font-size: 20px;
font-weight: bold;
color: #3f4042;
margin-left: 40px;
margin-bottom:60px ;
display: inline;        
}
span{
  font-size: 16px;
  font-weight: bold;
  color: #3f4042;
}
.icon-avatar{
    width: 50px;
    height: 50px;
    margin-left: 70px;
    margin-bottom: 10px;
}
</style>