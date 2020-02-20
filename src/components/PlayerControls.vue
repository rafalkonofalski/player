<template>
  <div class="player-controls">
    <PlayerControlsButton>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="13px"
        height="13px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(96, 85, 143)"
          d="M10.200,7.899 C9.547,7.899 8.958,8.172 8.539,8.609 L5.070,6.875 C5.089,6.754 5.100,
          6.629 5.100,
          6.500 C5.100,6.371 5.089,6.246 5.069,6.125 L8.539,4.391 C8.958,4.828 9.547,5.102 10.200,
          5.102 C11.470,
          5.102 12.500,4.070 12.500,2.801 C12.500,1.531 11.470,0.500 10.200,0.500 C8.930,0.500 7.900,
          1.531 7.900,
          2.801 C7.900,2.930 7.911,3.051 7.930,3.176 L4.461,4.910 C4.042,4.473 3.453,4.199 2.800,
          4.199 C1.530,
          4.199 0.500,5.231 0.500,6.500 C0.500,7.770 1.530,8.801 2.800,8.801 C3.453,8.801 4.042,
          8.527 4.461,
          8.090 L7.930,9.824 C7.911,9.950 7.900,10.074 7.900,10.199 C7.900,11.469 8.930,
          12.500 10.200,
          12.500 C11.470,12.500 12.500,11.469 12.500,10.199 C12.500,8.930 11.470,
          7.899 10.200,7.899 Z"
        />
      </svg>
    </PlayerControlsButton>
    <PlayerControlsButton mode="dark">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="13px"
        height="13px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(255, 255, 255)"
          d="M2.881,6.500 L12.500,0.500 L12.500,12.500 L2.881,6.500 ZM0.500,12.477 L0.500,0.500 L2.881,0.500 L2.881,6.500 L2.881,12.477 L0.500,12.477 Z"
        />
      </svg>
    </PlayerControlsButton>
    <PlayerControlsButton
      mode="dark"
      size="big"
      class="play"
      @buttonClicked="isPlaying = !isPlaying"
    >
      <svg
        v-if="isPlaying"
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        version="1.1"
        width="17"
        height="17"
        viewBox="0 0 17 17"
      >
        <path d="M152.443 136.417l207.114 119.573-207.114 119.593z" fill="#fff" />
      </svg>
      <svg
        v-else
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="17px"
        height="17px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(255, 255, 255)"
          d="M10.633,16.500 L10.633,0.500 L16.500,0.500 L16.500,16.500 L10.633,16.500 ZM0.500,0.500 L6.367,0.500 L6.367,16.500 L0.500,16.500 L0.500,0.500 Z"
        />
      </svg>
    </PlayerControlsButton>
    <PlayerControlsButton mode="dark">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="13px"
        height="13px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(255, 255, 255)"
          d="M10.118,12.500 L10.118,6.500 L10.118,0.522 L12.500,0.522 L12.500,12.500 L10.118,12.500 ZM0.500,0.500 L10.118,6.500 L0.500,12.500 L0.500,0.500 Z"
        />
      </svg>
    </PlayerControlsButton>
    <PlayerControlsButton>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="15px"
        height="12px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(237, 94, 116)"
          d="M14.497,3.805 C14.429,1.705 12.816,-0.000 10.743,-0.000 C9.360,-0.000 8.152,0.757 7.500,
          1.883 C6.848,0.757 5.640,-0.000 4.257,-0.000 C2.183,-0.000 0.570,1.705 0.503,3.805 C0.347,
          8.566 7.500,12.000 7.500,12.000 C7.500,12.000 14.652,8.566 14.497,3.805 Z"
        />
      </svg>
    </PlayerControlsButton>
    {{ isPlaying }}
  </div>
</template>

<script>
import PlayerControlsButton from "./PlayerControlsButton.vue";

export default {
  name: "PlayerControls",
  components: {
    PlayerControlsButton
  },
  data: () => ({
    isPlaying: false
  }),
  methods: {
    setState(e) {
      this.isPlaying = e;
    }
  }
};
</script>

<style lang="scss">
.player-controls {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 35px 30px 0;
}
</style>
