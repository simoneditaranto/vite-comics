<script>

export default{
    name: 'AppIcons',

    data() {
        return{

            iconCards: [
                {
                    iconImg: '/img/buy-comics-digital-comics.png',
                    iconTitle: 'digital comics',
                },
                {
                    iconImg: '/img/buy-comics-merchandise.png',
                    iconTitle: 'dc merchandise',
                },
                {
                    iconImg: '/img/buy-comics-subscriptions.png',
                    iconTitle: 'subscription',
                },
                {
                    iconImg: '/img/buy-comics-shop-locator.png',
                    iconTitle: 'comic shop locator',
                },
                {
                    iconImg: '/img/buy-dc-power-visa.svg',
                    iconTitle: 'dc power visa',
                },
            ]

        }
    }
}

</script>

<template>

    <div id="icons">

        <div class="cards">

            <div class="card" v-for="currentCard in iconCards">
                <img :src="currentCard.iconImg" alt="">
                <div class="icon-text">
                    {{ currentCard.iconTitle }}
                </div>
            </div>

        </div>


    </div>

</template>

<style lang="scss">

#icons{

    padding: 50px 0;

    background-color: #0282F9;

    .cards {
        display: flex;
        justify-content: center;
        gap: 70px;

        .card{
            display: flex;
            align-items: center;
            gap: 15px;

            img{
                width: 50px;
                height: 50px;
                object-fit: contain;
            }

            .icon-text {
                color: white;

                text-transform: uppercase;
            }
        }
    }
}

</style>