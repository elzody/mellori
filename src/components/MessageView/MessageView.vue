<script setup lang="ts">
import { ref } from 'vue'
import Message from './Message.vue'

const messages = ref([
  'I am the master of the C.L.I.T. Remember this fucking face.',
  'Kill yourself',
  ':3',
  'hab u seen an alien plz??',
  'KYS (Keep Yourself Safe) :D'
]);
</script>

<template>
  <div id="message-view">
    <Message v-for="msg in messages" :msg="msg" />
  </div>
</template>

<style>
  #message-view {
    display: flex;
    flex-flow: column nowrap;
    justify-content: end;
    font-size: 18px;
    color: var(--fg-3);
    background-color: var(--bg-2);
  }
</style>