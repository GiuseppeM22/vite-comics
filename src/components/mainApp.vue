<script>

import cardsApp from './cardsApp.vue'


export default {
    props: {
        images: Object
    },

    components: {
        cardsApp,
    },
    data() {
        return {
            icons: [
                {
                    name: 'DIGITAL COMICS',
                    path: '/assets/img/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    path: '/assets/img/buy-comics-merchandise.png'
                },
                {
                    name: 'SUBSCRIPTION',
                    path: '/assets/img/buy-comics-shop-locator.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    path: '/assets/img/buy-comics-subscriptions.png'
                },
                {
                    name: 'DC POWER VISA',
                    path: '/assets/img/buy-dc-power-visa.svg'
                }
            ]


        }
    }
}

</script>

<template>
    <!-- sezione colore nero -->
    <section class="bg_black">
        <div class="boxed boxedMain">
            <h3> -- Content goes here -- </h3>

            <cardsApp />
        </div>
    </section>
    <!-- sezione colore blue -->
    <section class="bg_blue">
        <div class="boxed icon flex">
            <div class="iconImg flex" v-for="icon in icons">
                <img :src="icon.path" alt="">
                <span>{{ icon.name }}</span>
            </div>
        </div>
    </section>
    <!-- sezione background immagine -->
    <section class="bg_image">
        <div class="boxed boxSpace flex">
            <div class="infos flex">
                <div class="leftInfo mr_30">
                    <div class="Comicsinfo">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li>Characters</li>
                            <li>Characters</li>
                            <li>Characters</li>
                            <li>Characters</li>
                            <li>Characters</li>
                            <li>Characters</li>
                        </ul>
                    </div>
                    <div class="shopInfo">
                        <h3>SHOP</h3>
                        <ul>
                            <li>Characters</li>
                            <li>Characters</li>
                        </ul>
                    </div>
                </div>
                <div class="DCinfo mr_30">
                    <h3>DC</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>
                <div class="SiteInfo">
                    <h3>SITES</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>
            </div>
            <div class="bigLogoImg">
                <img src="public/assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </section>
</template>

<style scoped>
.bg_black {
    background-color: #1c1c1c;
}

.bg_blue {
    background-color: #0282f9;
    z-index: 999;
    position: relative;
}

.boxedMain {
    color: white;
    padding: 40px;
}

.icon {
    padding: 40px;
    justify-content: space-around;
}

.iconImg {
    align-items: center;
}

.iconImg img {
    max-width: 35px;
    align-self: center;
}

.iconImg span {
    font-size: 12px;
    color: white;
    margin-left: 10px;
}

.bg_image {
    background-image: url(../assets/img/footer-bg.jpg);
    width: 100%;
    position: relative;
    height: 370px;
}

.infos {
    max-width: 50%;
    justify-content: space-between;
    padding: 40px 0;
}

.infos li {
    list-style-type: none;
    color: white;
    margin-top: 7px;
    font-size: 12px;
    color: #999;
}

.infos h3 {
    color: white;
    margin-top: 20px;
    margin-bottom: 10px;
}

.boxSpace {
    justify-content: space-between;
}

.bigLogoImg {
    position: absolute;
    transform: translate(+100%, -10%);
    margin-top: -50px;
    z-index: 2;
}
</style>
