<template>
  <div>
    <el-menu default-active="2" class="el-menu-vertical-demo" :collapse="isCollapse" @open="handleOpen" @close="handleClose" >
      <el-menu-item style="text-align: center;font-size: large">
        <NuxtLink to="/">< 退出</NuxtLink>
      </el-menu-item>
      <div class="flex items-center ml-8 mt-4 mb-4" >
        <span data-v-14565bac="" class="el-avatar el-avatar--circle" style="--el-avatar-size: 48px;">
      <img src="/assets/user.jpg" style="object-fit: cover;" alt="">
      </span>
        <div data-v-14565bac="" class="ml-4 flex flex-col max-w-[130px]">
          <span data-v-14565bac="" class="el-text is-truncated font-bold !self-baseline"><font _mstmutation="1" _msttexthash="6109597" _msthash="2302">小铭</font></span>
          <span data-v-14565bac="" class="el-text el-text--info is-truncated !self-baseline"><font _mstmutation="1" _msttexthash="5969067" _msthash="2301">管理</font></span>
        </div>
      </div>
      <el-menu-item :index="item.number" v-for="(item, index) in ListData" :key="index" @click="GetcomName(item.number)">
        <div>
          <img :src="item.url" alt="">
        </div>
        <template #title>{{item.name}}</template>
      </el-menu-item>
    </el-menu>
    <div class="window" >
      <component :is="ListData[comName].component"/>
    </div>
  </div>
</template>

<style>
.el-menu-vertical-demo:not(.el-menu--collapse) {
  width: 200px;
  min-height: 400px;
}
.window{
  width: 84%;
  height: 100%;
  position: absolute;
  right: 0;
  //background-color: blue;
  top: 0;
}
</style>

<script setup>
import User from '/assets/Like/user.svg'
import Setting from '/assets/Like/Setting.svg'
import Secure from '/assets/Like/Secure.svg'
import Account from '/assets/Like/Account.svg'

import Wes from "~/components/My/Wes.vue";
import Settings from "~/components/My/Settings.vue";
import Secures from "~/components/My/Secures.vue";
import Accounts from "~/components/My/Accounts.vue";

definePageMeta({
  layout: false,
})
const ListData = ref([
  {url: User ,name:'个人信息',number:'1',path: 'Wes',component:Wes},
  {url:Setting,name:'偏好设置',number:'2',path:'Settings',component:Settings},
  {url:Secure,name:'安全日志',number:'3',path: 'Secures',component:Secures},
  {url:Account,name:'账号管理',number:'4',path:'Accounts',component:Accounts},
])
const isCollapse = ref(false)
const path=ref('')
const comName= ref(1)
const GetcomName=(number)=>{
  comName.value=number-1
  return comName.value
}

</script>
