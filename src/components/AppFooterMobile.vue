<template>
    <div class="app__footer">
        <div class="footer">
            <div class="footer__logo">
                <img src="Star 1.svg" alt="footer_logo" class="footer_logo_pic">
                <p class="footer__sitename">Ink. House</p>
            </div>
            <div class="phone__text">
                <p class="phone">+7 (999) 543-54-54</p>
                <p class="workshop">Мастерская</p>
            </div>
            <div class="links__reproductions links">
                <h3 class="footer__header">Репродукции</h3>
                <p class="footer__country footer__nav">Франция</p>
                <p class="footer__country footer__nav">Германия</p>
                <p class="footer__country footer__nav">Англия</p>
            </div>
            <div class="links__new links">
                <h3 class="footer__header">Новинки</h3>
                <p class="footer__year footer__nav">2021</p>
                <p class="footer__year footer__nav">2020</p>
            </div>
            <div class="links__about links">
                <h3 class="footer__header">О нас</h3>
                <p class="footer__employee footer__nav">Художники</p>
                <p class="footer__employee footer__nav">Менеджеры</p>
            </div>
            <hr class="footer__spliter">
            <div class="footer__social">
                <div class="social__medias">
                    <img src="facebook.svg" alt="facebook" class="media">
                    <img src="instagram.svg" alt="instagram" class="media">
                    <img src="youtube.svg" alt="youtube" class="media">
                </div>
                <div class="social__rights">
                    <p class="rights__copy">Ink. House®</p>
                    <p class="rights__reserved">All rights reserved</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.app__footer {
    width: 100%;
    margin-top: 70px;
    background-color: #E1EDE6;
}

.footer {
    max-width: 290px;
    margin: 0 auto;
    padding: 23px 15px;
    align-content: flex-start;
    justify-content: center;
    justify-items: flex-start;
    display: grid;
    grid-template-columns: 143px 107px;
    grid-template-rows: 35px 109px 83px 1px 48px;
    gap: 20px 40px;
    font-family: Raleway;
}

.footer__phone {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.footer__logo {
    display: flex;
    align-items: center;
    grid-column: 1;
    grid-row: 1;
    gap: 8px;
}

.footer_logo_pic {
    width: 35px;
    height: 35px;
}

.footer__sitename {
    font-size: 20px;
    font-weight: 700;
    line-height: 23.48px;
    color: #598D66;
}

.phone__text {
    grid-column: 1 / 2;
    grid-row: 2 / 5;
}

.links__reproductions {
    grid-column: 2 / 2;
    grid-row: 2 / 5;
}

.links__new {
    grid-column: 1 / 2;
    grid-row: 3 / 5;
}

.links__about {
    grid-column: 2 / 2;
    grid-row: 3 / 5;
}

.phone__text {
    display: flex;
    flex-direction: column;
    gap: 8px;
    font-size: 16px;
    font-weight: 500;
    line-height: 18.78px;
    color: #2C2D35;
}

.workshop {
    font-size: 16px;
    font-weight: 500;
    line-height: 18.78px;
    color: #86928B;
}

.links {
    display: flex;
    flex-direction: column;
    gap: 6px;
}

.footer__header {
    font-size: 16px;
    font-weight: 500;
    line-height: 18.78px;
}

.footer__nav {
    font-size: 16px;
    font-weight: 500;
    line-height: 24px;
    color: #86928B;
}

.footer__spliter {
    height: 1px;
    width: 100%;
    background-color: #C3D1C6;
    grid-column-start: 1;
    grid-column-end: span 2; 
    grid-row: 4 / 5;
}

.footer__social {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
    justify-self: center;
    grid-column-start: 1;
    grid-column-end: span 2;
    grid-row: 5 / 5;
}

.social__medias {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 132px;
}

.media {
    width: 24px;
    height: 24px;
}

.social__rights {
    display: flex;
    align-items: center;
    font-size: 12px;
    font-weight: 500;
    line-height: 14.4px;
    color: #86928B;
}

@font-face {
    font-family: Raleway;
    src: url('/public/fonts/Raleway-VariableFont_wght.ttf');
}

</style>