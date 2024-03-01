<script>

export default {

    name: 'AppNav',

    data() {
        return {
            
            navLinks: [
                'characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop'
            ]
    
        }
    }

}


</script>

<template>
    
    <nav>

        <div class="container">
            
            <img src="/img/dc-logo.png" alt="dc logo">

            <ul>

                <li v-for="currentLink in navLinks">
                    {{ currentLink }}
                </li>

            </ul>

        </div>
        
    </nav>

</template>

<style lang="scss">

@use '../styles/mixins' as *;

nav{

    background-color: white;

    .container{
        @include centered-between;

        img{
            width: 80px;
            height: 80px;
        }

        ul{
            display: flex;
            gap: 30px;

            list-style-type: none;

            li{
                font-size: bold;

                text-transform: uppercase;
            }
        }
    }
    
}

.container{
    padding: 20px 0;
    margin: 0 auto;

    max-width: 1250px;
}
</style>