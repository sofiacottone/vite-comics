<script>
export default {
    components: {
        name: 'AppMainPages'
    }
}
</script>

<template>
    <section class="">
        <div class="container h-100">
            <div class="d-flex justify-content-center align-items-center text-white h-100">
                <ul class="d-flex gap-4 mb-0 ps-0 text-uppercase">
                    <li class="d-flex align-items-center">
                        <div class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </div>
                        <div class="ms-2">digital comics</div>
                    </li>
                    <li class="d-flex align-items-center">
                        <div class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-merchandise.png" alt="">
                        </div>
                        <div class="ms-2">dc merchandise</div>
                    </li>
                    <li class="d-flex align-items-center">
                        <div class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-subscriptions.png" alt="">
                        </div>
                        <div class="ms-2">subscription</div>
                    </li>
                    <li class="d-flex align-items-center">
                        <div class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-shop-locator.png" alt="">
                        </div>
                        <div class="ms-2">comic shop locator</div>
                    </li>
                    <li class="d-flex align-items-center">
                        <div class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-dc-power-visa.svg" alt="">
                        </div>
                        <div class="ms-2">dc power visa</div>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

section {
    background-color: $primary-color;
    height: 160px;
}

ul {

    .ms-img-container {
        display: inline-block;
        width: 60px;

        img {
            object-fit: contain;
            aspect-ratio: 3/2;
        }
    }
}

@media screen and (max-width: 1199px) {
    ul {
        li {
            flex-direction: column;
            text-align: center;

            .ms-img-container {
                padding-bottom: 10px;
            }
        }
    }
}
</style>