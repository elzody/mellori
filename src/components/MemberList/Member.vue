<template>
  <div class="member">
    <img src="/vite.svg" alt="Member profile image" />
    <div>
      <div>Username</div>
      <div>Write a status message</div>
    </div>
  </div>
</template>

<style>
  .member {
    display: flex;
    color: var(--fg-2);
    border-radius: 0.25rem;
    margin: 2px 5px;
    padding: 5px;

    & img {
      align-self: center;
      border-radius: 50%;
      width: 30px;
      margin: 5px;
      background-color: white;
    }

    & div {
      font-size: 12px;
      padding: 0px 2px;
    }

    & div:first-child {
      font-size: 15px;
    }
  }

  .member:hover {
    background-color: var(--bg-3);
    cursor: pointer;
  }
</style>