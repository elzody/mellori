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

<style>
  .channel {
    display: flex;
    align-items: center;
    margin: 2px 5px;
    padding: 2px;
    border-radius: 0.25rem;

    & svg {
      margin: 5px;
    }
  }

  .channel:hover {
    background-color: var(--bg-3);
    color: var(--fg-3);
    cursor: pointer;
  }
</style>