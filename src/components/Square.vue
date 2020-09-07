<template>
  <div>
    <div class="square" @click='claimTile()'>
      Click here
      <img v-if='isClaimed' :src="imageSource">
      <div v-if='isClaimed'>Claimed!</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Tile',
  data() {
    return {
      imageSource: '',
      claimedBy: '',
    }
  },
  computed: {
    isClaimed() {
      return this.claimedBy !== '';
    },
  },
  methods: {
    claimTile() {
      let color = 'RED';
      if (color.toUpperCase().includes('RED')) {
        this.imageSource = '../src/resources/red_x.png';
      } else {
        this.imageSource = '';
      }
      this.claimedBy = color;
    },
    getImageURL() {
      return this.imageSource;
    }
  },
}
</script>

<style scoped>
  .square {
    background-color: green;
    width: 10em;
    height: 10em;
  }
</style>