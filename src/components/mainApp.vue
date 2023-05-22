<script>

import cardsApp from './cardsApp.vue'


export default {
    components: {
        cardsApp,
    },
    data() {
        return {
            images: [
                {
                    thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book",
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book",
                },
                {
                    thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel",
                },
                {
                    thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book",
                },
                {
                    thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel",
                },
            ],
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
    <section>
        <div class="jumbo">
            <img src="public/assets/img/jumbotron.jpg" alt="">
            <button>CURRENT SERIES</button>
        </div>
    </section>
    <section class="bg_black">
        <div class="boxed boxedMain">

            <cardsApp :images="images" />
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
    display: flex;
    flex-wrap: wrap;

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

.jumbo {
    max-width: 100%;
    height: 30rem;
    position: relative;
}

.jumbo img {
    width: 100%;
    display: block;
    object-fit: cover;
    object-position: top;
    height: 100%;

}

.jumbo button {
    background-color: #0282f9;
    color: white;
    border: none;
    padding: 10px;
    font-size: 20px;
    font-weight: 800;
    position: absolute;
    left: 180px;
    top: 460px;
    cursor: pointer;
}
</style>
