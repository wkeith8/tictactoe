<template>
  <div>
    <img v-if='isClaimed' src='' onClick='claimTile'>
  </div>
</template>

<script>
export default {
  name: 'Board',
  data: {
    return: {
      playerImage: '',
    }
  },
  computed: {
    isClaimed: false,
  },
  methods: {
    claimTile(color) {
      if (color.toUpperCase().contains('RED')) {
        imageSource = '../src/resources/red_x.png';
      } else {
        imageSource = '';
      }
      isClaimed = true;
    }
  },
}
</script>