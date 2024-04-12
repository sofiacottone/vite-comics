<script>
export default {
    components: {
        name: 'AppMainCards'
    }
}
</script>

<template>
    <section class="container-fluid d-flex align-items-end">
        <div class="container position-relative">
            <div class="position-absolute text-uppercase text-white fw-bold h4 py-2 px-3">
                current series
            </div>
        </div>
    </section>
    <section class="bg-dark pt-5">
        <div class="container">
            <div class="d-flex flex-wrap">
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>

                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>
                <div class="ms-single-card ms-4">
                    <div class="ms-img-wrapper">
                        <img class="img-fluid" src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
                    </div>
                    <div class="text-uppercase text-white py-3">testo</div>
                </div>

            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

section {

    &.container-fluid {
        min-height: 400px;
        background-image: url(../assets/img/jumbotron.jpg);
        background-repeat: no-repeat;
        background-size: cover;

        .container {
            &>.position-absolute {
                background-color: $primary-color;
                width: fit-content;
                bottom: -30px;
            }

        }

    }

    &.bg-dark {
        height: fit-content;

        .ms-single-card {
            width: calc(100% / 6 - 1.5rem);
            margin-block: 20px;

            .ms-img-wrapper {
                img {
                    aspect-ratio: 1;
                    object-fit: cover;
                    object-position: top;
                }
            }
        }
    }

}

.bg-dark {
    width: 100%;
    height: 150px;
}
</style>