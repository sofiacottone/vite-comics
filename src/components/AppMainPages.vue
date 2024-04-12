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
                <ul class="d-flex gap-4 mb-0 text-uppercase">
                    <li>
                        <span class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </span>
                        <span class="ms-2">testo</span>
                    </li>
                    <li>
                        <span class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </span>
                        <span class="ms-2">testo</span>
                    </li>
                    <li>
                        <span class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </span>
                        <span class="ms-2">testo</span>
                    </li>
                    <li>
                        <span class="ms-img-container">
                            <img class="img-fluid" src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </span>
                        <span class="ms-2">testo</span>
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
        width: 50px;
    }
}
</style>