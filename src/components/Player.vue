<template>
  <div class="player">
    <PlayerHeader />
    <PlayerSongCover />
    <PlayerControlsVolume />
    <PlayerControls />
  </div>
</template>

<script>
// import axios from 'axios';
import PlayerHeader from './PlayerHeader.vue';
import PlayerSongCover from './PlayerSongCover.vue';
import PlayerControlsVolume from './PlayerControlsVolume.vue';
import PlayerControls from './PlayerControls.vue';

export default {
  name: 'Player',
  components: {
    PlayerHeader,
    PlayerSongCover,
    PlayerControlsVolume,
    PlayerControls,
  },

  // created() {
  //   axios.get('http://18.185.121.3:5000')
  //   .then(function (response) {
  //     console.log(response);
  //   })
  //   .catch(function (error) {
  //     console.log(error);
  //   });
  // }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.player {
  width: 360px;
  height: 480px;
  background-color: #eeeff5;
  border-radius: 26px;
  overflow: hidden;
  position: relative;
}
</style>
