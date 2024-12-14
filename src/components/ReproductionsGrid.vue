<template>
    <div class="reproductions">
        <p v-if="!reproductions">Загрузка...</p>
        <div v-else>
            <div class="reproductions__filters">
                <h2 class="reproduction__header">Репродукции</h2>
                <div class="reproduction__countries">
                    <button class="reproduction__country button" v-for="(item, key) in reproductions" :key="key"
                        @click="changeReproduction(item)">{{ item.Country }}</button>
                </div>
            </div>
            <div class="reproductions__grid">
                <PictureCard v-for="(picture, index) in pictures" :key="index" :picture-data="picture" />
            </div>
        </div>
    </div>
</template>
<script>
import PictureCard from './PictureCard.vue';

export default {
    data() {
        return {
            reproductions: null,
            pictures: null
        }
    },
    methods: {
        changeReproduction(item) {
            this.pictures = item.Reproductions;
        }
    },
    mounted() {
        fetch("reproductions.json")
        .then(resp => resp.json())
        .then(json => {
            this.reproductions = json;
            this.pictures = this.reproductions.France.Reproductions;
        });
    },
    components: {
        PictureCard
    }
}
</script>

<style>
.reproductions__filters {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    max-width: 1110px;
    margin: 0 auto 30px;
}

.reproduction__header {
    font-family: Raleway;
    font-size: 40px;
    font-weight: 500;
    line-height: 44px;
    color: #2C2D35;
}

.reproduction__countries {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    overflow-x: scroll;
    gap: 0 32px;
}

.reproduction__countries::-webkit-scrollbar {
    width: 0;
}

.reproduction__country.button {
    border: none;
    padding: 10px 20px;
    background-color: #D4E8D9;
    color: #2C2D35;
    border-radius: 20px;
    font-family: Raleway;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
}

.reproductions__grid {
    display: grid;
    max-width: 1110px;
    grid-template-columns: repeat(3, 350px);
    grid-template-rows: repeat(2, 730px);
    justify-content: center;
    align-items: center;
    justify-items: center;
    gap: 30px;
    margin: 0 auto;
}

@media screen and (width <= 1025px) {
    .reproductions__filters {
        max-width: 690px;
        padding: 0 39px;
    }

    .reproduction__header {
        font-size: 30px;
        font-weight: 500;
        line-height: 33px;
    }

    .reproduction__country.button {
        font-size: 20px;
        font-weight: 500;
        line-height: 23.48px;
    }

    .reproductions__grid {
        max-width: 690px;
        grid-template-columns: repeat(2, 330px);
        grid-template-rows: repeat(3, 730px);
    }
}

@media screen and (width <= 577px) {
    .reproductions__filters {
        max-width: 510px;
        padding: 0 33px;
        margin: 0 auto 20px;
    }

    .reproduction__header {
        font-size: 24px;
        font-weight: 500;
        line-height: 26.4px;
        margin: 20px inherit;
    }

    .reproduction__country.button {
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }

    .reproductions__grid {
        max-width: 510px;
        grid-template-columns: repeat(2, 240px);
        grid-template-rows: repeat(3, 514px);
    }
}

@media screen and (width <= 431px) {
    .reproductions__filters {
        max-width: 290px;
        padding: 0 15px;
    }

    .reproduction__header {
        font-size: 24px;
        font-weight: 500;
        line-height: 26.4px;
    }

    .reproduction__countries {
        gap: 0 20px;
    }

    .reproduction__country.button {
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }

    .reproductions__grid {
        max-width: 510px;
        grid-template-columns: repeat(1, 290px);
        grid-template-rows: repeat(6, 514px);
    }
}

@font-face {
    font-family: Raleway;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>