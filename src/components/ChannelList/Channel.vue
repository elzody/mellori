<script setup lang="ts">
import { ChannelType } from '../../types.ts'
import { PhHash, PhSpeakerSimpleHigh } from '@phosphor-icons/vue'

interface ChannelProps {
  name: string,
  type: ChannelType,
}

const props = defineProps<ChannelProps>();
</script>

<template>
  <div class="channel">
    <PhHash v-if="props.type == ChannelType.Text" :size="22" weight="regular" />
    <PhSpeakerSimpleHigh v-else :size="22" weight="fill" />
    <div>{{ props.name }}</div>
  </div>
</template>

<style scoped>
  .channel {
    display: flex;
    flex-flow: row nowrap;
    align-items: center;
    text-overflow: ellipsis;
    margin: 2px 5px;
    border-radius: 0.25rem;
    color: #ADB5BD;
  }

  .channel:hover {
    background-color: #495057;
    color: #F8F9FA;
    cursor: pointer;
  }

  .channel svg {
    margin: 5px;
  }
</style>