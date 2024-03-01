<script>
import AppIcons from './AppIcons.vue';

export default{
    name: 'AppFooter',

    components: {
        AppIcons,
    },

    data() {

        return {
            footerLinks: [
                {
                    title: 'dc comics',
                    links: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ],
                },

                {
                    title: 'shop',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                },

                {
                    title: 'dc',
                    links: [
                        'Terms Of Use',
                        'Privacy policy (new)',
                        'Terms Of Use',
                        'Privacy policy',
                        'Terms Of Use',
                        'Privacy policy',
                        'Terms Of Use',
                        'Privacy policy',
                        'Terms Of Use',
                        'Privacy policy',
                        'Terms Of Use',
                    ],
                },

                {
                    title: 'sites',
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC',
                        'MAD Magazine',
                        'DC',
                    ],
                },
            ]
        }

    }
}

</script>

<template>

    <footer>
        <AppIcons></AppIcons>

        <div class="container">
            
            <div class="links">

                <div 
                    class="link-list" 
                    v-for="currentElement in footerLinks"
                >
                    <h3>{{ currentElement.title }}</h3>
                    <ul>
                        <li v-for="currentLink in currentElement.links">
                            {{ currentLink }}
                        </li>
                    </ul>
                </div>

            </div>

            
            <img src="/img/dc-logo-bg.png" alt="">
            
        </div>
        
    </footer>

</template>

<style lang="scss">
@use '../styles/mixins' as *;

footer{

    background-image: url('/img/footer-bg.jpg');
    background-size: cover;

    .container{
        @include centered-between;

        height: 400px;

        overflow: hidden;

        padding: 0;

        color: white;

        .links{
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            gap: 10px 40px;

            padding: 40px 0;

            height: 100%;
        }

        h3{
            margin-bottom: 10px;

            text-transform: uppercase;
        }

        ul{
            list-style-type: none;

            li{
                color: #959595;

                cursor: pointer;

                &:hover{
                    color: white;

                    text-decoration: underline;
                }
            }
        }

    }

}

</style>