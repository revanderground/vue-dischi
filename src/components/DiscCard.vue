<template>
       
    <div class="disc-card text-center m-2">
        <img class="image-album" :src="image" >
        <div class="title pt-2">{{title}}</div>
        <div class="info">{{author}}</div>
        <div class="info">{{year}}</div>

    </div>

</template>

<script>
export default {
    name: 'discCard',
    props: ['image', 'title', 'author', 'year']
}
</script>

<style lang="scss" scoped>
    .disc-card{
        background-color: #2E3A46;
        width:calc((100% / 5) - 1rem);
        height: 18rem;
        padding: 1rem;
    }
    
    .image-album{
        width: 90%;
    }

    .title{
        font-size: 0.9rem;
        text-transform: uppercase;
        font-weight: 600;
    }

    .info{
        font-size: 0.8rem;
        color:#b0a69f;
    }



</style>