<template lang="pug">
h1 吉他社社史
input(
type="button"
  value="社團介紹" @click="goto('/')")
input(
type="button"
  value="活動公告" @click="goto('/guitar/events')")
input(
type="button"
  value="教學內容" @click="goto('/guitar/teach')")
</template>

<script setup>
import { useRouter } from 'vue-router'
// router 是可以操作使用者連結的變數
// route 是取得目前路由資訊的變數
const router = useRouter()
const goto = (path) => {
  router.push(path)
}
</script>
