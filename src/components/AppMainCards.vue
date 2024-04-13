<script>
import SingleCard from './SingleCard.vue';

export default {
    name: 'AppMainCards',
    components: {
        SingleCard
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://comichub.blob.core.windows.net/high/0d5eb026-ee1c-468f-b5ca-af1d5ace57e2.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://comichub.blob.core.windows.net/low/766a10bc-e558-4e1b-acec-0361fde8a658.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://comichub.blob.core.windows.net/low/a8221777-17ea-4ba4-82ad-f3ed9f0a6bc6.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/I/41nGyVF7C2L.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://comichub.blob.core.windows.net/low/db33b8a5-17b3-42eb-90d7-43f3702d358f.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i.ebayimg.com/images/g/YgYAAOSwu0BfjPo5/s-l1200.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://mycomics.it/wp-content/uploads/sites/16/2022/12/FUMCAWOPA0008.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
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
            <!-- cards  -->
            <div class="d-flex flex-wrap">
                <SingleCard v-for="comic in comics" :cardInfo="comic"></SingleCard>
            </div>
            <div class="d-flex justify-content-center mt-4 pb-3">
                <div class="ms-btn text-uppercase text-white fw-bold py-2 px-5">
                    load more
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
    }

}

.bg-dark {
    width: 100%;
    height: 150px;

    .ms-btn {
        background-color: $primary-color;
        width: fit-content;
        cursor: pointer;
    }
}
</style>