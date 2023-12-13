<script setup lang="ts">

</script>

<template>
  <div class="message">
    <img src="/vite.svg" alt="User icon" />
    <div>
      <span>User name</span>
      <p>
        I am the master of the C.L.I.T. Remember this fucking face.
      </p>
    </div>
  </div>
</template>

<style scoped>
  .message {
    display: flex;
    color: #F8F9FA;
  }

  .message img {
    align-self: flex-start;
    flex-basis: 48px;
    flex-shrink: 0;
    border-radius: 50%;
  }

  .message div {
    display: flex;
    flex-flow: column nowrap;
  }

  .message div > * {
    margin: 0;
    padding: 0;
  }

  .message div span {
  }

  .message div p {
  }
</style>