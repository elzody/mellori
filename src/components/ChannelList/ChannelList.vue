<script setup lang="ts">
import Channel from './Channel.vue'
import { ChannelType } from '../../types.ts'
</script>

<template>
  <div id="channel-list">
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

<style>
  #channel-list {
    background-color: var(--bg-1);
    display: flex;
    flex-flow: column nowrap;
    width: 225px;
    font-size: 15px;
    color: var(--fg-2);
  }
</style>