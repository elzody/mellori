<script setup lang="ts">
import { PhPlusCircle } from '@phosphor-icons/vue'
</script>

<template>
  <div id="message-input-bar">
    <div>
      <PhPlusCircle :size="32" weight="fill" />
      <input type="text" placeholder="Send message in #channel-name" />
    </div>
  </div>
</template>

<style>
  #message-input-bar {
    background-color: var(--bg-2);
    padding: 10px 10px 20px 10px;

    & div {
      display: flex;
      align-items: center;
      column-gap: 5px;
      background-color: var(--bg-4);
      padding: 5px;
      border-radius: 0.25rem;

      & svg:hover {
        cursor: pointer;
      }

      & input {
        background-color: rgba(255, 255, 255, 0);
        outline: 0;
        border: 0;
        flex: 1 1 auto;
        color: var(--fg-3);
        padding: 5px;
        font-size: 18px;
        font-family: 'Noto Sans', sans-serif;
      }
    }
  }
</style>