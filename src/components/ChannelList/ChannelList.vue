<script setup lang="ts">
import TextChannel from "./TextChannel.vue"
</script>

<template>
  <div id="channelList">
    <TextChannel name="general" />
    <TextChannel name="memes" />
  </div>
</template>

<style scoped>
  #channelList {
    background-color: #343A40;
    display: flex;
    flex-flow: column nowrap;
    width: 200px;
    font-size: 15px;
  }
</style>