<template>
  <div id="app">
    <Header1 />

    <main>
      <DiscList />
    </main>

  </div>   

</template>

<script>
import Header1 from './components/Header.vue'
import DiskAlbum from './components/DiskAlbum.vue'
import DiskCard from './components/DiskCard.vue'



export default {
  name: 'App',
  components: {
    Header1,
    DiskAlbum,
    DiskCard,
    
}
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import '@/assets/scss/style.scss';



</style>
