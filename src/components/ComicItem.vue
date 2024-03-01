<script>

export default {
    name: 'ComicItem',

    // dichiaro le proprietà del mio item
    props: {
        // titolo della serie
        comicSeries: String,
        // url dell'immagine
        comicImage: String,
    }
}

</script>

<template>

    <div class="comic-card">
        <div class="comic-img">
            <img :src="comicImage" alt="">
        </div>
        <span>{{ comicSeries }}</span>
    </div>

</template>

<style lang="scss">

.comic-card{

    width: calc(100% / 6 - 25px / 6 * 5);

    .comic-img {

        margin-bottom: 10px;

        width: 100%;
        
        img{
            width: 100%;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: top;
        }

    }


    span{
        color: white;

        text-transform: uppercase;
    }
}

</style>