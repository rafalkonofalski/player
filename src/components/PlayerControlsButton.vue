<template>
  <a class="player-controls-button" :class="[mode, size]">
    <slot></slot>
  </a>
</template>

<script>
export default {
  props: {
    mode: {
      type: String,
      default: 'light'
    },
    
    size: {
      type: String,
      default: 'normal'
    }
  },

  name: 'PlayerControlsButton',
};
</script>

<style lang="scss">
  .player-controls-button {
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    background-color: rgb(255, 255, 255);
    width: 36px;
    height: 36px;

    &.dark {
      background-color: #60558f;
    }

    &.big {
      width: 50px;
      height: 50px;
    }
  }
</style>
