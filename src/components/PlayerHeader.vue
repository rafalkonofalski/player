<template>
  <div class="player__header player-control">
    <a href="#" class="player-control__item">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="17px"
        height="17px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(255, 255, 255)"
          d="M16.397,7.230 L13.898,7.230 C13.996,7.645 14.047,8.073 14.047,
          8.509 C14.047,9.258 13.900,9.983 13.611,10.664 C13.332,11.324 12.932,
          11.917 12.422,12.427 C11.911,12.935 11.318,13.336 10.658,13.615 C9.976,
          13.903 9.250,14.049 8.500,14.049 C7.750,14.049 7.023,13.903 6.342,
          13.615 C5.682,13.336 5.088,12.935 4.577,12.427 C4.067,11.917 3.667,
          11.324 3.388,10.664 C3.100,9.983 2.953,9.258 2.953,8.509 C2.953,
          7.759 3.100,7.034 3.388,6.352 C3.667,5.693 4.067,5.100 4.577,
          4.591 C5.088,4.081 5.682,3.680 6.342,3.402 C7.023,3.113 7.750,
          2.968 8.500,2.968 C9.250,2.968 9.976,3.113 10.658,3.402 C10.948,
          3.524 11.225,3.671 11.488,3.839 L9.923,5.402 L14.830,5.402 L14.830,
          0.500 L13.250,2.078 C11.922,1.097 10.278,0.516 8.500,0.516 C4.081,
          0.516 0.500,4.095 0.500,8.509 C0.500,12.922 4.081,16.500 8.500,
          16.500 C12.918,16.500 16.500,12.922 16.500,8.509 C16.500,
          8.073 16.465,7.646 16.397,7.230 Z"
        ></path>
      </svg>
    </a>
    <a href="#" class="player-control__item">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="17px"
        height="16px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(255, 255, 255)"
          d="M3.969,13.120 L3.969,15.279 L0.500,11.857 L3.969,8.436 L3.969,
          10.595 L13.939,10.595 L13.939,8.813 L16.500,6.289 L16.500,10.595 L16.500,
          12.526 L16.500,13.120 L3.969,13.120 ZM13.030,4.967 L3.060,4.967 L3.060,
          6.748 L0.500,9.273 L0.500,2.442 L13.030,2.442 L13.030,0.284 L16.500,
          3.704 L13.030,7.126 L13.030,4.967 Z"
        ></path>
      </svg>
    </a>
    <a href="#" class="player-control__item">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="17px"
        height="16px"
      >
        <path
          fill-rule="evenodd"
          fill="rgb(255, 255, 255)"
          d="M16.498,3.818 L13.029,7.259 L13.029,5.087 L10.072,5.087 L8.592,
          2.549 L13.029,2.549 L13.029,0.378 L16.498,3.818 ZM13.018,10.662 L13.018,
          8.491 L16.487,11.931 L13.018,15.372 L13.018,13.200 L9.226,13.200 L9.226,
          13.198 L9.223,13.200 L4.500,5.087 L0.502,5.087 L0.502,2.549 L5.972,
          2.549 L5.972,2.553 L5.977,2.549 L10.701,10.662 L13.018,10.662 ZM6.606,
          13.200 L0.502,13.200 L0.502,10.662 L5.125,10.662 L6.606,13.200 Z"
        ></path>
      </svg>
    </a>
    <a href="#" class="player-control__item player-control__item--hamburger">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="17px"
        height="14px"
      >
        <path
          fill-rule="evenodd"
          opacity="0.302"
          fill="rgb(255, 255, 255)"
          d="M0.500,13.681 L0.500,11.084 L16.500,11.084 L16.500,13.681 L0.500,
          13.681 ZM0.500,5.889 L16.500,5.889 L16.500,8.486 L0.500,8.486 L0.500,
          5.889 ZM0.500,0.693 L16.500,0.693 L16.500,3.291 L0.500,3.291 L0.500,
          0.693 Z"
        ></path>
      </svg>
    </a>
  </div>
</template>

<script>
export default {
  name: 'PlayerHeader',
};
</script>

<style lang="scss" scoped>
  .player {
    &__header {
      background-color: rgba(42,34,77,0.6);
      display: flex;
      align-items: center;
      justify-content: center;
      position: absolute;
      left: 0;
      top: 0;
      z-index: 1;
      width: 100%;
      height: 65px;
    }

    &-control {
      &__item {
        margin: 0 12px;

        &--hamburger {
          position: absolute;
          top: 23px;
          right: 10px;
        }
      }
    }
  }
</style>
