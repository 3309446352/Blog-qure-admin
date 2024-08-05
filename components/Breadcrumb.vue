<template>
  <div class="Breadcrumb">
    <div class="grid-container">
      <div></div>
      <div class="item"><h1>首页</h1></div>
      <div class="item-2"></div>
      <div><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" class="globalization navbar-bg-hover w-[40px] h-[48px] p-[11px] cursor-pointer outline-none el-tooltip__trigger el-tooltip__trigger" role="img" width="1em" height="1em" viewBox="0 0 24 24" style="outline: none;"><path fill="currentColor" d="m18.031 16.617l4.283 4.282l-1.415 1.415l-4.282-4.283A8.96 8.96 0 0 1 11 20c-4.968 0-9-4.032-9-9s4.032-9 9-9s9 4.032 9 9a8.96 8.96 0 0 1-1.969 5.617Zm-2.006-.742A6.977 6.977 0 0 0 18 11c0-3.867-3.133-7-7-7s-7 3.133-7 7s3.133 7 7 7a6.977 6.977 0 0 0 4.875-1.975l.15-.15Z"></path></svg></div>
      <div><svg data-v-9119df37="" xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" aria-hidden="true" class="globalization navbar-bg-hover w-[40px] h-[48px] p-[11px] cursor-pointer outline-none el-tooltip__trigger el-tooltip__trigger" viewBox="0 0 512 512" id="header-translation" role="button" tabindex="0" aria-controls="el-id-304-62" aria-expanded="false" aria-haspopup="menu"><path fill="currentColor" d="m478.33 433.6-90-218a22 22 0 0 0-40.67 0l-90 218a22 22 0 1 0 40.67 16.79L316.66 406h102.67l18.33 44.39A22 22 0 0 0 458 464a22 22 0 0 0 20.32-30.4zM334.83 362 368 281.65 401.17 362zm-66.99-19.08a22 22 0 0 0-4.89-30.7c-.2-.15-15-11.13-36.49-34.73 39.65-53.68 62.11-114.75 71.27-143.49H330a22 22 0 0 0 0-44H214V70a22 22 0 0 0-44 0v20H54a22 22 0 0 0 0 44h197.25c-9.52 26.95-27.05 69.5-53.79 108.36-31.41-41.68-43.08-68.65-43.17-68.87a22 22 0 0 0-40.58 17c.58 1.38 14.55 34.23 52.86 83.93.92 1.19 1.83 2.35 2.74 3.51-39.24 44.35-77.74 71.86-93.85 80.74a22 22 0 1 0 21.07 38.63c2.16-1.18 48.6-26.89 101.63-85.59 22.52 24.08 38 35.44 38.93 36.1a22 22 0 0 0 30.75-4.9z"></path></svg></div>
      <div><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" class="globalization navbar-bg-hover w-[40px] h-[48px] p-[11px] cursor-pointer outline-none el-tooltip__trigger el-tooltip__trigger" role="img" width="1em" height="1em" viewBox="0 0 24 24" style="outline: none;"><path fill="currentColor" d="M16 3h6v6h-2V5h-4V3ZM2 3h6v2H4v4H2V3Zm18 16v-4h2v6h-6v-2h4ZM4 19h4v2H2v-6h2v4Z"></path></svg></div>
      <div><svg data-v-1760ac04="" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="globalization navbar-bg-hover w-[40px] h-[48px] p-[11px] cursor-pointer outline-none el-tooltip__trigger el-tooltip__trigger" aria-hidden="true" role="img" width="1em" height="1em" viewBox="0 0 1024 1024" style="outline: none;"><path fill="currentColor" d="M512 64a64 64 0 0 1 64 64v64H448v-64a64 64 0 0 1 64-64z"></path><path fill="currentColor" d="M256 768h512V448a256 256 0 1 0-512 0v320zm256-640a320 320 0 0 1 320 320v384H192V448a320 320 0 0 1 320-320z"></path><path fill="currentColor" d="M96 768h832q32 0 32 32t-32 32H96q-32 0-32-32t32-32zm352 128h128a64 64 0 0 1-128 0z"></path></svg></div>
      <div class="globalization navbar-bg-hover w-[60px] h-[48px] p-[11px]">
        <div class="we-icon-1">小铭</div>
      </div>
      <div class="globalization navbar-bg-hover w-[40px] h-[48px] p-[11px]">
        <el-popover :visible="visible" placement="bottom" title=""  content="">
          <template #reference>
            <el-avatar :size="25" ><img src="../assets/user.jpg" alt=""></el-avatar>
          </template>
          <el-button style="text-align: center">
            <h1  @click="My">账户设置</h1>
          </el-button>
        </el-popover>
      </div>

      <div><svg data-v-9119df37="" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="globalization navbar-bg-hover w-[40px] h-[48px] p-[11px] cursor-pointer outline-none el-tooltip__trigger el-tooltip__trigger" aria-hidden="true" role="img" width="1em" height="1em" viewBox="0 0 24 24" style="outline: none;"><path fill="currentColor" d="M3.34 17a10.017 10.017 0 0 1-.979-2.326a3 3 0 0 0 .003-5.347a9.99 9.99 0 0 1 2.5-4.337a3 3 0 0 0 4.632-2.674a9.99 9.99 0 0 1 5.007.003a3 3 0 0 0 4.632 2.671a10.056 10.056 0 0 1 2.503 4.336a3 3 0 0 0-.002 5.347a9.99 9.99 0 0 1-2.501 4.337a3 3 0 0 0-4.632 2.674a9.99 9.99 0 0 1-5.007-.002a3 3 0 0 0-4.631-2.672A10.018 10.018 0 0 1 3.339 17Zm5.66.196a4.992 4.992 0 0 1 2.25 2.77c.499.047 1 .048 1.499.002a4.993 4.993 0 0 1 2.25-2.772a4.993 4.993 0 0 1 3.526-.564c.29-.408.54-.843.748-1.298A4.993 4.993 0 0 1 18 12c0-1.26.47-2.437 1.273-3.334a8.152 8.152 0 0 0-.75-1.298A4.993 4.993 0 0 1 15 6.804a4.993 4.993 0 0 1-2.25-2.77c-.5-.047-1-.048-1.5-.001A4.993 4.993 0 0 1 9 6.804a4.993 4.993 0 0 1-3.526.564c-.29.408-.54.843-.747 1.298A4.993 4.993 0 0 1 6 12c0 1.26-.471 2.437-1.273 3.334a8.16 8.16 0 0 0 .75 1.298A4.993 4.993 0 0 1 9 17.196ZM12 15a3 3 0 1 1 0-6a3 3 0 0 1 0 6Zm0-2a1 1 0 1 0 0-2a1 1 0 0 0 0 2Z"></path></svg></div>
    </div>
    <div class="dao-2">
      <el-breadcrumb separator="/">
        <el-breadcrumb-item :to="{ path: '/' }"><h1>首页</h1></el-breadcrumb-item>
        <el-breadcrumb-item><h1>异常页面</h1>
        </el-breadcrumb-item>
        <el-breadcrumb-item :to="{ path: '/Error' }">403</el-breadcrumb-item>
        <el-breadcrumb-item :to="{ path: '/Error' }">404</el-breadcrumb-item>
      </el-breadcrumb>
    </div>
  </div>
</template>

<style lang="less">
.grid-container{
  display: flex;
  justify-content:flex-end;
  height: 50px;
  .item{
    padding:10px 0
  }
  .item-2 {
    flex-grow: 2;
  }
  .we-iocn-1{
    display:inline;
    width: 50px;
  }
}
.dao-2{
  height: 30px;
  //background-color: aquamarine;
}
</style>
<script lang="ts" setup>
defineComponent({
  name: "Breadcrumb"
})

const state = reactive({
  circleUrl:
    'https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png',
  squareUrl:
    'https://cube.elemecdn.com/9/c2/f0ee8a3c7c9638a54940382568c9dpng.png',
  sizeList: ['small', '', 'large'] as const,
})
const { circleUrl, squareUrl, sizeList } = toRefs(state)
const router = useRouter()
const My = () => {
    router.push('/login')
  }
</script>