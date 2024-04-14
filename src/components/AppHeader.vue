<script>
export default {
    components: {
        name: 'AppHeader'
    },
    data() {
        return {
            activeItem: 0,
            headerNavLinks: [
                {
                    "name": "characters",
                    "active": false,
                },
                {
                    "name": "comics",
                    "active": true,
                },
                {
                    "name": "movies",
                    "active": false,
                },
                {
                    "name": "tv",
                    "active": false,
                },
                {
                    "name": "games",
                    "active": false,
                },
                {
                    "name": "collectibles",
                    "active": false,
                },
                {
                    "name": "videos",
                    "active": false,
                },
                {
                    "name": "fans",
                    "active": false,
                },
                {
                    "name": "news",
                    "active": false,
                },
                {
                    "name": "shop",
                    "active": false,
                }
            ],
            scrollPosition: 0,
        }
    },
    methods: {
        changeActiveItem(clickedIndex) {
            this.activeItem = clickedIndex;
        },
        updateScroll() {
            this.scrollPosition = window.scrollY;
        }
    },
    mounted() {
        window.addEventListener('scroll', () => { this.updateScroll() });
    }
}
</script>

<template>
    <header class="bg-light position-fixed w-100">

        <nav class="navbar navbar-expand-lg bg-body-tertiary p-0">
            <div class="container">
                <img :class="[scrollPosition >= 20 ? 'logo-small' : '']" src="../assets/img/dc-logo.png" alt="DC Logo">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                    <!-- navbar links -->
                    <div v-for="(link, index) in headerNavLinks" class="navbar-nav text-uppercase ms-auto">
                        <a :class="{ 'active': index == activeItem }, [scrollPosition >= 20 ? 'nav-small' : 'h-130']"
                            class="nav-link d-flex align-items-center" @click="changeActiveItem(index)" href="#">{{
                    link.name }}</a>
                    </div>
                </div>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

header {
    overflow: hidden;
    transition: 0.4s;
    top: 0;
    z-index: 100;
}

.navbar-nav {

    .nav-link {
        color: #464646;
        font-weight: bold;
        border-bottom: 4px solid transparent;
        position: relative;

        &.active {
            color: $primary-color;
            border-bottom: 4px solid $primary-color;
        }
    }
}

// resize navbar 
.h-130 {
    height: 130px;
}

.nav-small {
    height: 70px;
}

.logo-small {
    height: 50px;
}

// responsive 
@media screen and (max-width: 991px) {
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