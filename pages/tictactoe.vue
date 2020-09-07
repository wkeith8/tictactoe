<template>
  <Square/>
</template>

<script>
  import Square from '../src/components/Square.vue';

  export default {
    components: {
      Square
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