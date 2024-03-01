<script>

export default {
    name: 'AppJumbo',
}

</script>

<template>

    <div class="jumbo-img">
        <img src="/img/jumbotron.jpg" alt="">
    </div>

</template>

<style lang="scss">

.jumbo-img{
    width: 100%;
    height: 400px;
    
    img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
}


</style>