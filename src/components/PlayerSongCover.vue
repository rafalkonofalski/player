<template>
  <div
    class="player__cover"
    style="background-image: url('https://bi.im-g.pl/im/29/ab/14/z21672489V,W-Gdansku-rozpoczal-sie-jeden-z-najpopularniejszyc.jpg)"
  >
    <PlayerSongDetails />
  </div>
</template>

<script>
import PlayerSongDetails from "./PlayerSongDetails.vue";

export default {
  name: "PlayerSongCover",
  components: {
    PlayerSongDetails
  }
};
</script>

<style lang="scss">
.player {
  &__cover {
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: 100%;
    max-height: 360px;
    position: relative;
  }
}
</style>
