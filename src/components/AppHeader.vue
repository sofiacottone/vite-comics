<script>
export default {
    components: {
        name: 'AppHeader'
    }
}
</script>

<template>
    <header class="bg-light">

        <nav class="navbar navbar-expand-lg bg-body-tertiary">
            <div class="container">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                    <div class="navbar-nav ms-auto text-uppercase">
                        <a class="nav-link active" aria-current="page" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                        <a class="nav-link" href="#">link</a>
                    </div>
                </div>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/generic' as *;

header {
    height: 130px;
}

.navbar-nav {

    .nav-link {
        color: #464646;
        font-weight: bold;
        border-bottom: 2px solid transparent;
        position: relative;
        height: 3rem;

        &.active {
            color: $primary-color;
        }

        &.active::after {
            content: "";
            position: absolute;
            bottom: -48px;
            left: 0;
            right: 0;
            height: 4px;
            background-color: $primary-color;
        }
    }
}
</style>