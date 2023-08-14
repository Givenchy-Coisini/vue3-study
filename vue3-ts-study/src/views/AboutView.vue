<!--
 * @Author: fuyongjie
 * @Date: 2023-08-09 21:44:09
 * @Description: 文件描述~
 * @FilePath: /vue3-study/vue3-ts-study/src/views/AboutView.vue
 * @LastEditTime: 2023-08-14 12:06:53
 * @LastEditors: fuyongjie
-->
<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<script setup lang="ts">
import { useRoute, useRouter } from 'vue-router';

const route = useRoute()
const router = useRouter()

console.log('dddd', route.params === router.currentRoute.value.params)
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
