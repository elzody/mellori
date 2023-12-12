<script setup lang="ts">
import ServerListIcon from './ServerListIcon.vue';
</script>

<template>
  <div id="serverListSidebar">
    <ServerListIcon />
    <ServerListIcon />
    <ServerListIcon />
    <ServerListIcon />
    <ServerListIcon />
    <ServerListIcon />
  </div>
</template>

<style scoped>
#serverListSidebar {
  background-color: #212529;
  display: flex;
  flex-flow: column nowrap;
}
</style>
