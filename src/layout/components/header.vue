<script setup>
import {ref} from 'vue'
import {useRouter} from 'vue-router'
const router = useRouter()

const menuList = ref([{
  name:'首页',
  path:'/'
},{
  name:'关于',
  path:'/about'
},{
  name:'登录',
  path:'/login'
}])
const handle = (path) => {
  router.push(path)
}
</script>

<template>
  <div class="header">
    到焊条
    <div class="menu" >
      <ul style="display: flex;">
        <li style="margin-right: 50px;" v-for="(item,index) in menuList" :key="index" @click="handle(item.path)">{{item.name}}</li>
      </ul>
  </div>
  </div>
</template>``

<style scoped>
.header {
    width:100%;
    background: red;
}
</style>
