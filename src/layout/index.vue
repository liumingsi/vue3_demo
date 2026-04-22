<script setup>

import Header from './components/header.vue'
import Selse from './components/selse.vue'
</script>

<template>
  <div class="box">
    <Header/>
    <Selse/>
  </div>
</template>

<style scoped>
.box {
    width:100%;
    height: calc(100% - 100px);
}
</style>