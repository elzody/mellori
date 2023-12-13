<script setup lang="ts">
import ServerListIcon from './ServerListIcon.vue';
</script>

<template>
  <div>
    <ServerListIcon v-for="num in 3" />
  </div>
</template>

<style scoped>
  div {
    background-color: #212529;
    display: flex;
    flex-flow: column nowrap;
  }
</style>
