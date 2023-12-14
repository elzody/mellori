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
    padding: 5px 10px;
    margin: 5px 0;

    & img {
      align-self: flex-start;
      width: 40px;
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