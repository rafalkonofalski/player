<template>
  <a class="player-controls-button" :class="[mode, size]" @click.prevent="$emit('buttonClicked')">
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
    cursor: pointer;
    position: relative;

    &.dark {
      background-color: #60558f;
    }

    &.big {
      width: 50px;
      height: 50px;
    }

    &.play {
      width: 64px;
      height: 64px;
      background-color: #fff;

      &::before {
        content: '';
        display: block;
        position: absolute;
        left: 2px;
        top: 2px;
        width: calc(100% - 4px);
        height: calc(100% - 4px);
        background: conic-gradient(lightgray 0deg, lightgray 60deg, white 60deg, white 360deg);
        border-radius: 50%;

      }

      &::after {
        content: '';
        display: block;
        position: absolute;
        left: 7px;
        top: 7px;
        width: calc(100% - 14px);
        height: calc(100% - 14px);
        background-color: #60558f;
        border-radius: 50%;
        z-index: 0;
      }

      svg {
        z-index: 1;
      }
    }
  }
</style>
