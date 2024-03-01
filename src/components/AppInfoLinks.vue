<script>

export default{
    name: 'AppInfoLinks',

    data() {
        return {

            socials: [
                {
                    socialName: 'facebook',
                    socialIcon: '/img/footer-facebook.png',
                },
                {
                    socialName: 'twitter',
                    socialIcon: '/img/footer-twitter.png',
                },
                {
                    socialName: 'youtube',
                    socialIcon: '/img/footer-youtube.png',
                },
                {
                    socialName: 'pinterest',
                    socialIcon: '/img/footer-pinterest.png',
                },
                {
                    socialName: 'periscope',
                    socialIcon: '/img/footer-periscope.png',
                },
            ]

        }
    }
}

</script>

<template>

    <div id="info-links">

        <div class="container">

            <button>Sing up now!</button>

            <div class="socials">
                <div class="follow-us">follow us</div>
                <img
                    v-for="currentSocial in socials" 
                    :src="currentSocial.socialIcon" :alt="currentSocial.socialName"
                >
                
            </div>

        </div>

    </div>

</template>

<style lang="scss">

@use '../styles/variables' as *;
@use '../styles/mixins' as *;

#info-links{
    background-color: #303030;

    .container{
        @include centered-between;

        padding: 30px 0;

        button{
            padding: 18px;

            text-transform: uppercase;

            border: 2px solid $myBlueColor;

            background-color: #303030;
            
            cursor: pointer;
        }

        .socials{
            display: flex;
            align-items: center;
            gap: 30px;

            .follow-us{
                font-weight: bold;
    
                text-transform: uppercase;

                color: $myBlueColor;
            }

            img{

               cursor: pointer;

               &:hover{
                   filter: invert(100%);
               }

            }
        }
    }
}
</style>