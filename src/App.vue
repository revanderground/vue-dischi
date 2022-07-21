<template>
  <div id="app">
    <Header1 />

    <main>
      <DiscAlbum />
    </main>

  </div>   

</template>

<script>
import Header1 from './components/Header.vue'
import DiscAlbum from './components/DiscAlbum.vue'
import DiscCard from './components/DiscCard.vue'



export default {
  name: 'App',
  components: {
    Header1,
    DiscAlbum,
    DiscCard,

}
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import '@/assets/scss/style.scss';



</style>
