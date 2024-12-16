<template>
    <div class="hero">
        <img src="bird.png" alt="hero" class="hero__picture">
        <div class="hero__about">
            <h1 class="about__header">
                Реплики картин от <span class="Ink__house">Ink. House</span>
            </h1>
            <p class="about__paragraph">
                Высокое качество отрисовки на плотной бумаге или льняном холсте. Редкие произведения, доступные цены.
            </p>
            <a class="about__production button" href="#">Продукция</a>
        </div>
    </div>
    <ReproductionsGrid />
    <PromoCollection />
    <OurTeam />
</template>

<style>
.hero {
    display: flex;
    align-items: center;
    justify-content: center;
    max-width: 1110px;
    margin: 0 auto;
    padding: 0 15px;
    gap: 30px;
}

.hero__picture {
    width: 540px;
    height: 621px;
}

.hero__about {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    font-family: Raleway;
    text-align: left;
}

.about__header {
    font-size: 60px;
    font-weight: 500;
    line-height: 66px;
    color: #2C2D35;
    margin-bottom: 20px;
}

.Ink__house {
    color: #598D66;
}

.about__paragraph {
    font-size: 18px;
    font-weight: 500;
    line-height: 27px;
    color: #86928B;
    margin-bottom: 60px;
}

.about__production.button {
    display: flex;
    justify-content: center;
    align-items: center;
    text-decoration: none;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    color: #598D66;
    border: 1px solid #598D66;
    background-color: transparent;
    width: 225px;
    height: 65px;
    cursor: pointer;
}

.about__production.button:hover {
    background-color: #EEDB6D;
    color: #2C2D35;
}

.about__production.button:active {
    background-color: #D9B949;
    color: #2C2D35;
}

@media screen and (width <= 769px) {
    .hero {
        padding: 0 39px;
    }
    .hero__picture {
        width: 330px;
        height: 380px;
    }

    .about__header {
        font-size: 40px;
        font-weight: 500;
        line-height: 40px;
    }

    .about__paragraph {
        margin-bottom: 40px;
    }

    .about__production.button {
        width: 210px;
        height: 60px;
    }
}

@media screen and (width <= 577px) {
    .hero {
        margin-top: 50px;
        padding: 0 33px;
    }

    .hero__picture {
        width: 195px;
        height: 239px;
    }

    .about__header {
        font-size: 36px;
        font-weight: 500;
        line-height: 36px;
        margin-bottom: 10px;
    }

    .about__paragraph {
        font-size: 16px;
        font-weight: 500;
        line-height: 24px;
        margin-bottom: 11px;
    }

    .about__production.button {
        width: 178px;
        height: 50px;
        font-family: Raleway;
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }
}

@media screen and (width <= 376px) {
    .hero {
        margin-top: 60px;
        padding: 0 15px;
    }

    .hero__picture {
        display: none;
    }

    .about__header {
        font-size: 30px;
        font-weight: 500;
        line-height: 30px;
        margin-bottom: 20px;
    }

    .about__paragraph {
        font-size: 14px;
        font-weight: 500;
        line-height: 21px;
        margin-bottom: 40px;
    }

    .about__production.button {
        width: 154px;
        height: 50px;
    }
}

@font-face {
    font-family: Raleway;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>

<script>
import PromoCollection from '@/components/PromoCollection.vue';
import ReproductionsGrid from '@/components/ReproductionsGrid.vue';
import OurTeam from '@/components/OurTeam.vue';


export default {
    data() {
        return {

        }
    },
    components: {
        ReproductionsGrid,
        PromoCollection,
        OurTeam
    }
}

</script>