<script setup lang="ts">
import { PhHash } from '@phosphor-icons/vue';

interface TextChannelProps {
  name: string,
}

const props = defineProps<TextChannelProps>();
</script>

<template>
  <div id="channelListItem">
    <PhHash :size="22" weight="regular" />
    <div>{{ props.name }}</div>
  </div>
</template>

<style scoped>
  #channelListItem {
    display: flex;
    flex-flow: row nowrap;
    align-items: center;
    text-overflow: ellipsis;
    margin: 2px 5px;
    border-radius: 0.25rem;
    color: #ADB5BD;
  }

  #channelListItem:hover {
    background-color: #495057;
    color: #F8F9FA;
    cursor: pointer;
  }

  #channelListItem svg {
    margin: 5px;
  }
</style>