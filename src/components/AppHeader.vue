<script>
export default {
    components: {
        name: 'AppHeader'
    }
}
</script>

<template>
    <header class="bg-light">

        <nav class="navbar navbar-expand-lg bg-body-tertiary p-0">
            <div class="container">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                    <!-- navbar links -->
                    <div class="navbar-nav text-uppercase ms-auto">
                        <a class="nav-link d-flex align-items-center" href="#">characters</a>
                        <a class="nav-link active d-flex align-items-center" href="#">comics</a>
                        <a class="nav-link d-flex align-items-center" href="#">movies</a>
                        <a class="nav-link d-flex align-items-center" href="#">tv</a>
                        <a class="nav-link d-flex align-items-center" href="#">games</a>
                        <a class="nav-link d-flex align-items-center" href="#">collectibles</a>
                        <a class="nav-link d-flex align-items-center" href="#">videos</a>
                        <a class="nav-link d-flex align-items-center" href="#">fans</a>
                        <a class="nav-link d-flex align-items-center" href="#">news</a>
                        <a class="nav-link d-flex align-items-center" href="#">shop</a>
                    </div>
                </div>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/generic' as *;

.navbar-nav {

    .nav-link {
        color: #464646;
        font-weight: bold;
        border-bottom: 4px solid transparent;
        position: relative;
        height: 130px;

        &.active {
            color: $primary-color;
            border-bottom: 4px solid $primary-color;
        }
    }
}

@media screen and (max-width: 960px) {
    .navbar-nav {
        margin-top: 10px;

        .nav-link {
            height: 50px;
        }
    }

    .navbar {
        img {
            margin-block: 10px
        }
    }
}
</style>