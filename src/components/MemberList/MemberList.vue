<script setup lang="ts">
import Member from './Member.vue'
</script>

<template>
  <div id="member-list">
    <Member v-for="num in 5" />
  </div>
</template>

<style>
  #member-list {
    display: flex;
    flex-flow: column nowrap;
    width: 225px;
    background-color: var(--bg-1);
  }
</style>