<template>
      <header>
        <nav class="navbar navbar-light">
            <nav class="navbar">
                <a class="navbar-brand" href="#">
                    
                    <img src="https://www.freepnglogos.com/uploads/spotify-logo-png/spotify-download-logo-30.png" alt="">
                </a>

            </nav>

                <div class="select-box float-right">
                    <select class="form-select" aria-label="Default select example">
                        <option selected>Scegli il Genere</option>
                        <option value="1">Rock</option>
                        <option value="2">Pop</option>
                        <option value="3">Jazz</option>
                        <option value="4">Metal</option>
                    </select>
                </div>
        </nav>
    </header>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    header{
        background-color: #2E3A46;
        padding: 0 1rem;
        a{
            width: 4rem;
            img{
                width: 100%;
            }
        }
    }

    .select-box{
        margin-right: 50px;
    }


</style>