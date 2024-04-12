<script>
export default {
    components: {
        name: 'AppContactsFooter'
    }
}
</script>

<template>
    <div class="container-fluid">
        <div class="container">
            <div class="d-flex justify-content-between py-5">
                <div>
                    <!-- sign up button  -->
                    <button class="text-uppercase text-white p-2">
                        <a href="">sign-up now!</a>
                    </button>
                </div>

                <!-- socials  -->
                <div class="d-flex align-items-center gap-4">
                    <h5 class="text-uppercase mb-0">follow us</h5>

                    <div>
                        <img class="pe-3" src="../assets/img/footer-facebook.png" alt="fb logo">
                        <img class="pe-3" src="../assets/img/footer-twitter.png" alt="twitter logo">
                        <img class="pe-3" src="../assets/img/footer-youtube.png" alt="youtube logo">
                        <img class="pe-3" src="../assets/img/footer-pinterest.png" alt="pinterest logo">
                        <img src="../assets/img/footer-periscope.png" alt="periscope logo">
                    </div>
                </div>

            </div>

        </div>

    </div>
</template>

<style lang="scss" scoped>
@use '../style/generic' as *;

.container-fluid {
    background-color: #303030;

    button {
        background: transparent;
        border: 2px solid $primary-color;
        ;
    }

    h5 {
        color: $primary-color;
    }
}
</style>