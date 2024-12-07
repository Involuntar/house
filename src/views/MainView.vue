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
            <button class="about__production button">Продукция</button>
        </div>
    </div>
    <ReproductionsGrid />
</template>

<style>
.hero {
    display: flex;
    align-items: center;
    justify-content: center;
    max-width: 1110px;
    margin: 0 auto;
    padding: 15px;
    gap: 30px;
}

.hero__picture {
    width: 540px;
    height: 621px;
}

.hero__about {
    display: flex;
    flex-direction: column;
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

@font-face {
    font-family: Raleway;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>

<script>
import ReproductionsGrid from '@/components/ReproductionsGrid.vue';


export default {
    data() {
        return {

        }
    },
    components: {
        ReproductionsGrid
    }
}

</script>