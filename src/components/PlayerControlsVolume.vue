<template>
  <div class="volume-control">
    <div class="volume-control__bar">
      <div class="volume-control__button" style="left: 50%">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          width="13px"
          height="10px"
        >
          <path
            fill-rule="evenodd"
            fill="rgb(96, 85, 143)"
            d="M11.111,7.902 L10.338,7.130 C10.670,6.764 10.933,6.346 11.119,
            5.883 C11.327,5.369 11.431,4.824 11.431,4.260 C11.431,3.697 11.327,
            3.150 11.119,2.635 C10.933,2.174 10.670,1.754 10.338,1.389 L11.111,
            0.615 C11.972,1.565 12.500,2.848 12.500,4.260 C12.500,5.670 11.972,
            6.953 11.111,7.902 ZM9.768,6.558 L8.995,5.785 C9.369,5.370 9.573,
            4.832 9.573,4.260 C9.573,3.687 9.369,3.148 8.995,2.733 L9.768,
            1.961 C10.309,2.560 10.642,3.369 10.642,4.260 C10.642,5.150 10.309,
            5.959 9.768,6.558 ZM3.794,2.343 L7.747,0.063 L7.747,9.062 L3.794,
            7.174 L3.794,2.343 ZM0.500,6.484 L0.500,3.034 C0.500,2.652 0.794,
            2.343 1.158,2.343 L3.135,2.343 L3.135,7.174 L1.158,7.174 C0.794,
            7.174 0.500,6.865 0.500,6.484 Z"
          />
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PlayerControlsVolume',
};
</script>

<style lang="scss">
  .volume-control {
    &__bar {
      height: 7px;
      background-color: #fff;
      position: relative;
    }

    &__button {
      width: 22px;
      height: 22px;
      border-radius: 50%;
      background-color: #fff;
      box-shadow: 1px 1px 3px rgba(0,0,0,0.4);
      display: flex;
      align-items: center;
      justify-content: center;
      position: absolute;
      transform: translate(-7px, -8px);
      cursor: pointer;

      &::before {
        content: '';
        display: block;
        position: absolute;
        left: 22px;
        height: 7px;
        width: 360px;
        background-color:#ed5e74;
      }
    }
  }
</style>
