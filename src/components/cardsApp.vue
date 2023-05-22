<script>
export default {
    props: {
        images: Object
    },
}

</script>


<template>
    <div v-for="card in images" class="card">
        <img :src="card.thumb" alt="">
        <span>{{ card.series }}</span>
    </div>
    <button class="load">LOAD MORE</button>
</template>

<style scoped>
.card {
    width: calc(100% / 6);
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
}

.card img {
    max-width: 150px;
    height: 200px;
    margin-bottom: 10px;
}

.card span {
    font-size: 12px;
}

.load {
    background-color: #0282f9;
    color: white;
    border: none;
    padding: 10px 35px;
    font-size: 16px;
    margin: auto;
    cursor: pointer;
}
</style>