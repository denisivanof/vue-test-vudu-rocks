<template>
  <article class="post">
    <h2 class="post__title">{{item.title}}</h2>
    <p class="post__body">{{item.body}}</p>
    <div class="post__user">{{item.username}}</div>
  </article>
</template>

<script setup lang="ts">
import type {Ipost} from "@/App.vue";
const props = defineProps<{
  item: Ipost
}>()
</script>

<style scoped lang="scss">
@import "../assets/post";
</style>
