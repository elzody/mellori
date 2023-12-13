<script setup lang="ts">
import Channel from './Channel.vue'
import { ChannelType } from '../../types.ts'
</script>

<template>
  <div>
    <Channel
      v-for="num in 5"
      :name="'text-channel-' + num.toString()"
      :type="ChannelType.Text"
    />

    <Channel
      v-for="num in 3"
      :name="'Voice ' + num.toString()"
      :type="ChannelType.Voice"
    />
  </div>
</template>

<style scoped>
  div {
    background-color: #343A40;
    display: flex;
    flex-flow: column nowrap;
    width: 200px;
    font-size: 15px;
  }
</style>