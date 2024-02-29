<script>

export default{
    name: 'AppFooter',

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

footer{

    background-image: url('/img/footer-bg.jpg');
    background-size: cover;

    .container{
        display: flex;
        justify-content: space-between;
        align-items: flex-start;

        color: white;

        .links{
            display: flex;
            gap: 55px;

            padding: 45px 0 0;
        }

        h3{
            margin-bottom: 20px;

            text-transform: uppercase;
        }

        ul{
            list-style-type: none;

            li{
                color: #959595;

                cursor: pointer;
            }
        }
    }

}
/* img{
    transform: translateY(-25%);
} */

</style>