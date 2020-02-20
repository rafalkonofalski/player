<template>
  <div class="player__details song">
    <div class="song__artist">Icona Pop</div>
    <div class="song__title">Still Don't Know</div>
  </div>
</template>

<script>
export default {
  name: "PlayerSongDetails"
};
</script>

<style lang="scss" scoped>
.player {
  &__details {
    background-color: rgba(42, 34, 77, 0.6);
    height: 65px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: absolute;
    left: 0;
    bottom: 0;
  }
}

.song {
  color: #ffffff;
  &__artist {
    font-size: 17px;
    font-weight: bold;
    margin-bottom: 4px;
  }

  &__title {
    font-size: 13px;
  }
}
</style>
