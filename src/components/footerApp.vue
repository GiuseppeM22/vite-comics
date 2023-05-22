<script>
</script>

<template>
    <section class="bg_gray">
        <div class="boxed flex">
            <div class="signIn">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="socials flex">
                <div class="follow">
                    <span>FOLLOW US</span>
                </div>
                <div class="socialImg">
                    <img src="public/assets/img/footer-facebook.png" alt="">
                    <img src="public/assets/img/footer-periscope.png" alt="">
                    <img src="public/assets/img/footer-pinterest.png" alt="">
                    <img src="public/assets/img/footer-twitter.png" alt="">
                    <img src="public/assets/img/footer-youtube.png" alt="">
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.bg_gray {
    background-color: #303030;
    padding-top: 30px;
    z-index: 999;
    position: relative;
    bottom: 0;
    right: 0;
    height: 100px;
    width: 100%;
}

.boxed {
    justify-content: space-between;
    align-items: center;
}

.signIn button {
    color: white;
    background-color: #303030;
    padding: 10px;
    cursor: pointer;
    border: 2px solid #303030;
}

.signIn button:hover {
    border: 2px solid #0282f9;

}

.socials {
    align-items: center;
}

.socials span {
    color: #0282f9;
    font-size: 16px;
    font-weight: 800;
}

.socials img {
    margin-left: 10px;
    max-width: 25px;
    cursor: pointer;
}
</style>
