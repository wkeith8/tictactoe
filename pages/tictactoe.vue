<template>
  <img src="../src/resources/red_x.png" class="board"/>
</template>

<script>
  import Tile from '../src/components/Tile.vue';

  export default {
    components: {
      Tile
    }
  }
</script>

<style scoped>
  .board {
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    width: 8em;
    color: red;
    font-size: 32px;
    object-position: 50% 50%;
    align-content: center;
  }
</style>