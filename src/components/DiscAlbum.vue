<template>
    <div id="disc-album" >
        <div class="disc-card-box mt-4 mb-5" v-if="albumsList">
            <DiscCard 
            v-for="(element, index) in albumsList"
            :key="index"
            :image="element.poster"
            :title="element.title"
            :author="element.author"
            :year="element.year"
            />


        </div>

        <div class="loader position-absolute top-50 start-50 translate-middle" v-else>
        <h3>Caricamento in corso...</h3>
        </div>

       
     
    </div>
</template>

<script>
import DiscCard from './DiscCard.vue';
import axios from 'axios';

export default {
    name: 'discAlbum',
    components: {
        DiscCard
    },

    data: function(){
        return {
            albumsList: null
        }
    },

    created(){
        setTimeout(this.apiGetAlbums, 3000);
    },
    
    methods: {
          apiGetAlbums(){
            axios.get('https://flynn.boolean.careers/exercises/api/array/music')
            .then((result) => {
                this.albumsList = result.data.response;
                console.log(this.almbumsList);
            })
        }
        
    }

}

</script>

<style lang="scss" scoped>
    #disc-album{
        width: 80%;
        height:600px;

        margin: 0 auto;
      
        .disc-card-box{
       
            display:flex;
            flex-wrap:wrap;


        }

    }

   


</style> 