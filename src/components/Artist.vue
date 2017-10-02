<template lang="html">
  <li class="artist">
    <h2><a v-bind:href="artist.url" target="_blank">{{artist.name}}</a></h2>
   <img :src="artist.image[2]['#text']" alt="">
 </li>
</template>

<script>
export default {
  name : 'artist',
  props: ['artist']


}
</script>

<style lang="css" scoped>
li.artist{
  display: block;
  margin: 10px 0;
}
</style>
