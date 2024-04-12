<script>
import AppContactsFooter from '../components/AppContactsFooter.vue';


export default {
    components: {
        name: 'AppFooter',
        AppContactsFooter,
    }
}
</script>

<template>
    <!-- main footer  -->
    <div class="container-fluid ms-bg-container">
        <div class="container">
            <div class="d-flex gap-5 py-5">

                <!-- first column  -->
                <div>
                    <div>
                        <h4 class="text-uppercase text-white">dc comics</h4>
                        <ul class="ps-0">
                            <li class="fw-normal">
                                <a href="">Characters</a>
                            </li>
                            <li class="fw-normal">
                                <a href="">Comics</a>
                            </li>
                            <li class="fw-normal">
                                <a href="">Movies</a>
                            </li>
                            <li class="fw-normal">
                                <a href="">TV</a>
                            </li>
                            <li class="fw-normal">
                                <a href="">Games</a>
                            </li>
                            <li class="fw-normal">
                                <a href="">Videos</a>
                            </li>
                            <li class="fw-normal">
                                <a href="">News</a>
                            </li>
                        </ul>
                    </div>

                    <div>
                        <h4 class="text-uppercase text-white">shop</h4>
                        <ul class="ps-0">
                            <li class="fw-normal">
                                <a href="">Shop DC</a>
                            </li>
                            <li class="fw-normal">
                                <a href="">Shop DC Collectibles</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <!-- second column  -->
                <div>
                    <h4 class="text-uppercase text-white">dc</h4>
                    <ul class="ps-0">
                        <li class="fw-normal">
                            <a href="">Terms of Use</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Privacy Policy (New)</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Ad Choices</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Advertising</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Jobs</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Subscriptions</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Talent Workshops</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">CPSC Certificates</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Ratings</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Shop Help</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">Contact Us</a>
                        </li>
                    </ul>
                </div>
                <!-- third column  -->
                <div>
                    <h4 class="text-uppercase text-white">sites</h4>
                    <ul class="ps-0">
                        <li class="fw-normal">
                            <a href="">DC</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">MAD Magazine</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">DC Kids</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">DC Universe</a>
                        </li>
                        <li class="fw-normal">
                            <a href="">DC Power Visa</a>
                        </li>
                    </ul>
                </div>

            </div>

        </div>
    </div>

    <!-- contacts  -->
    <AppContactsFooter></AppContactsFooter>
</template>

<style lang="scss" scoped>
@use '../style/generic' as *;

.ms-bg-container {
    min-height: 360px;
    width: 100%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

    .container {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;
    }
}

li {
    a {
        color: #5d5d5d;
        cursor: pointer;
    }
}
</style>