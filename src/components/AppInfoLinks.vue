<script>

export default{
    name: 'AppInfoLinks'
}

</script>

<template>

    <div id="info-links">

        <div class="container">

            <button>Sing up now!</button>

            <div class="socials">
                <div class="follow-us">follow us</div>
                <img src="/img/footer-facebook.png" alt="">
                <img src="/img/footer-twitter.png" alt="">
                <img src="/img/footer-youtube.png" alt="">
                <img src="/img/footer-pinterest.png" alt="">
                <img src="/img/footer-periscope.png" alt="">
            </div>

        </div>

    </div>

</template>

<style lang="scss">

#info-links{
    background-color: #303030;

    position: absolute;
    width: 100%;

    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;

        padding: 30px 0;

        button{
            padding: 18px;

            text-transform: uppercase;

            border: 2px solid #0282F9;

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

                color: #0282F9;
            }
        }
    }
}
</style>