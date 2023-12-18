<script setup lang="ts">
import { ref } from 'vue'
import Message from './Message.vue'
import InputBar from './InputBar.vue'

const messages = ref([
  'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
  'Velit egestas dui id ornare.',
  'Aliquet bibendum enim facilisis gravida neque.',
  'Scelerisque viverra mauris in aliquam sem fringilla ut. Augue mauris augue neque gravida in fermentum et sollicitudin.',
  'Pellentesque id nibh tortor id aliquet. Morbi tristique senectus et netus et malesuada.',
  'Non quam lacus suspendisse faucibus. Eu non diam phasellus vestibulum lorem sed risus ultricies. Gravida rutrum quisque non tellus. Magna etiam tempor orci eu lobortis elementum nibh.',
  'Tincidunt ornare massa eget egestas purus viverra. Urna neque viverra justo nec ultrices dui sapien eget mi.',
  'Aliquet bibendum enim facilisis gravida. Nam aliquam sem et tortor consequat id. Porttitor lacus luctus accumsan tortor posuere ac ut consequat. Elementum curabitur vitae nunc sed velit dignissim. Turpis nunc eget lorem dolor.',
  'Pretium quam vulputate dignissim suspendisse. Magna ac placerat vestibulum lectus mauris ultrices eros in cursus. Lobortis elementum nibh tellus molestie. Ipsum nunc aliquet bibendum enim.',
  'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
  'Velit egestas dui id ornare.',
  'Aliquet bibendum enim facilisis gravida neque.',
  'Scelerisque viverra mauris in aliquam sem fringilla ut. Augue mauris augue neque gravida in fermentum et sollicitudin.',
  'Pellentesque id nibh tortor id aliquet. Morbi tristique senectus et netus et malesuada.',
  'Non quam lacus suspendisse faucibus. Eu non diam phasellus vestibulum lorem sed risus ultricies. Gravida rutrum quisque non tellus. Magna etiam tempor orci eu lobortis elementum nibh.',
  'Tincidunt ornare massa eget egestas purus viverra. Urna neque viverra justo nec ultrices dui sapien eget mi.',
  'Aliquet bibendum enim facilisis gravida. Nam aliquam sem et tortor consequat id. Porttitor lacus luctus accumsan tortor posuere ac ut consequat. Elementum curabitur vitae nunc sed velit dignissim. Turpis nunc eget lorem dolor.',
  'Pretium quam vulputate dignissim suspendisse. Magna ac placerat vestibulum lectus mauris ultrices eros in cursus. Lobortis elementum nibh tellus molestie. Ipsum nunc aliquet bibendum enim.',
  'Velit egestas dui id ornare.',
  'Aliquet bibendum enim facilisis gravida neque.',
  'Scelerisque viverra mauris in aliquam sem fringilla ut. Augue mauris augue neque gravida in fermentum et sollicitudin.',
  'Pellentesque id nibh tortor id aliquet. Morbi tristique senectus et netus et malesuada.',
]);
</script>

<template>
  <div id="message-view">
    <div id="messages">
      <Message v-for="msg in messages" :msg="msg" />
    </div>

    <InputBar />
  </div>
</template>

<style>
  #message-view {
    display: flex;
    flex-flow: column nowrap;
    overflow-y: auto;
    font-size: 18px;
    color: var(--fg-3);
    background-color: var(--bg-2);
  }

  #messages {
    flex-grow: 1;
    display: flex;
    flex-flow: column nowrap;
    row-gap: 15px;
    overflow-y: auto;
  }
</style>