<script>

export default {
    data() {
        return {
            icons: [
                {
                    name: 'DIGITAL COMICS',
                    path: '../assets/img/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    path: '../assets/img/buy-comics-merchandise.png'
                },
                {
                    name: 'SUBSCRIPTION',
                    path: '../assets/img/buy-comics-shop-locator.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    path: '../assets/img/buy-comics-subscriptions.png'
                },
                {
                    name: 'DC POWER VISA',
                    path: '../assets/img/buy-dc-power-visa.svg'
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
        <div class="boxed"></div>
    </section>
</template>

<style scoped>
.bg_black {
    background-color: #1c1c1c;
}

.bg_blue {
    background-color: #0282f9;
}

.boxedMain {
    color: white;
    padding: 30px;
}

.icon {
    height: 200px;
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
</style>
