<script setup lang="ts">
interface MessageProps {
  msg: string,
}

const props = defineProps<MessageProps>();
</script>

<template>
  <div class="message">
    <img src="/vite.svg" alt="User icon" />
    <div>
      <div>Username</div>
      <div>{{ props.msg }}</div>
    </div>
  </div>
</template>

<style>
  .message {
    display: flex;
    padding: 5px;

    & img {
      align-self: flex-start;
      flex: 0 0 40px;
      margin-top: 5px; /* TODO: Find better way to align image with message author */
      border-radius: 50%;
      background-color: white;
    }

    & div {
      padding: 0 6px;
    }
  }

  .message:hover {
    background-color: var(--bg-3);
  }
</style>