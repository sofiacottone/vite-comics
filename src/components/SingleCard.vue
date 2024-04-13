<script>
export default {
    name: 'SingleCard',
    props: {
        cardInfo: Object
    },
    methods: {
        getImageUrl(name) {
            return new URL(`${name}`, import.meta.url).href
        }
    }
}
</script>

<template>

    <div class="ms-single-card col-xl-2 col-lg-3 col-md-4 col-sm-6 col-12">
        <div class="ms-img-wrapper">
            <img class="img-fluid" :src="getImageUrl(cardInfo.thumb)" :alt="cardInfo.series">
        </div>
        <div class="text-uppercase text-white pt-3 pe-3">{{ cardInfo.series }}</div>
    </div>

</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.ms-single-card {
    margin-block: 10px;

    .ms-img-wrapper {
        width: 170px;

        img {
            aspect-ratio: 1;
            object-fit: cover;
            object-position: top;
            width: 100%;
        }
    }
}

// responsive 
@media screen and (max-width: 966px) {
    .ms-single-card {
        .ms-img-wrapper {
            width: 190px;
        }
    }

}

@media screen and (max-width: 756px) {
    .ms-single-card {
        .ms-img-wrapper {
            width: 220px;
        }
    }

}

@media screen and (max-width: 573px) {
    .ms-single-card {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;

        .ms-img-wrapper {
            width: 320px;

        }

        div.text-uppercase {
            font-size: 25px;
        }
    }

}
</style>