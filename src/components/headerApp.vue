<script>

export default {
    data() {
        return {
            links: [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP',
            ]
        }
    }
}

</script>

<template>
    <section>
        <div class="boxed boxedHeader flex">
            <div class="logo">
                <img src="public/assets/img/dc-logo.png" alt="">
            </div>
            <div class="menu">
                <a v-for="link in links" href="">{{ link }}</a>
            </div>
        </div>
    </section>
</template>

<style scoped>
.boxedHeader {
    justify-content: space-between;
    align-items: center;
    padding: 10px;
}

.boxedHeader img {
    max-width: 70px;
}

.menu a {
    text-decoration: none;
    font-size: 13px;
    margin-right: 20px;
    color: #666;
    font-weight: 800;
}

.menu a:hover {
    color: #0282f9;
}
</style>
