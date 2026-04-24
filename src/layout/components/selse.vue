<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
  <div class="sidebar">
    <div class="select">
      <ul>
        <li>
          <div>
            1
          </div>
        </li>
        <li>
          <div>
            2
          </div>
        </li>
        <li>
          <div>
            3
          </div>
        </li>
        </ul>
    </div>
    <div class="main">
      <RouterView />
    </div>
  </div>
</template>

<style scoped>
.sidebar {
    width: 100%;
    height:100%;
    display: flex;
    /* 选择器样式 */
    .select {
        width: 100px;
        height: 100%;
        background-color: rgb(58, 176, 245);
    }
    .main {
        flex: 1;
        height: 100%;
    }
}
</style>
