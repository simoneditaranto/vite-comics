<script>

export default {

    name: 'AppNav',

    data() {
        return {
            
            navLinks: [
                'characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop'
            ],

            activeLinkIndex: 1,
    
        }
    }

}


</script>

<template>
    
    <nav>

        <div class="container">
            
            <img src="/img/dc-logo.png" alt="dc logo">

            <ul>

                <li 
                    v-for="(currentLink, index) in navLinks"
                    :class="index == activeLinkIndex ? 'active' : ''"
                >
                    {{ currentLink }}
                </li>

            </ul>

        </div>
        
    </nav>

</template>

<style lang="scss">
@use '../styles/variables' as *;
@use '../styles/mixins' as *;

nav{
    height: 120px;

    background-color: white;

    .container{
        @include centered-between;
        padding: 0;
        height: 100%;

        img{
            height: 80px;
        }

        ul{
            display: flex;
            align-items: stretch;
            gap: 30px;

            height: 100%;

            list-style-type: none;

            li{
                position: relative;
                display: flex;
                align-items: center;

                font-size: bold;

                text-transform: uppercase;

                cursor: pointer;

                &.active{
                    color: $myBlueColor;
                }

                &.active::before {
                    content: '';
                    position: absolute;
                    bottom: 0;
                    left: 0;

                    width: 100%;
                    height: 6px;

                    background-color: $myBlueColor;
                }
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