<script setup lang="ts">
import ServerListIcon from './ServerListIcon.vue';
</script>

<template>
  <div id="server-list">
    <ServerListIcon v-for="num in 3" />
  </div>
</template>

<style>
  #server-list {
    background-color: var(--bg-0);
    display: flex;
    flex-flow: column nowrap;
  }
</style>
