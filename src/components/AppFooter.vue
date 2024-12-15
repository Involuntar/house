<template>
    <div class="app__footer">
        <div class="footer">
            <div class="footer__phone">
                <div class="footer__logo">
                    <img src="Star 1.svg" alt="footer_logo" class="footer_logo_pic">
                    <p class="footer__sitename">Ink. House</p>
                </div>
                <div class="phone__text">
                    <p class="phone">+7 (999) 543-54-54</p>
                    <p class="workshop">Мастерская</p>
                </div>
            </div>
            <div class="footer__links">
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
    max-width: 1110px;
    margin: 0 auto;
    padding: 23px 15px;
    align-content: flex-start;
    display: grid;
    grid-template-columns: auto auto auto;
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
    display: flex;
    flex-direction: column;
    gap: 8px;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    color: #2C2D35;
}

.workshop {
    font-size: 18px;
    font-weight: 500;
    line-height: 21.13px;
    color: #86928B;
}

.footer__links {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}

.links {
    display: flex;
    flex-direction: column;
    gap: 6px;
}

.footer__header {
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
}

.footer__nav {
    font-size: 18px;
    font-weight: 500;
    line-height: 27px;
    color: #86928B;
}

.footer__spliter {
    display: none;
    width: 100%;
    margin: -14px 0;
    background-color: #C3D1C6;
}

.footer__social {
    display: flex;
    flex-direction: column;
    gap: 10px;
    justify-self: flex-end;
    width: 132px;
}

.social__medias {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.media {
    width: 24px;
    height: 24px;
}

.social__rights {
    font-size: 12px;
    font-weight: 500;
    line-height: 14.4px;
    color: #86928B;
}

@media screen and (width <= 769px) {
    .footer {
        max-width: 690px;
        grid-template-columns: repeat(2, auto);
        grid-template-rows: repeat(2, auto);
        gap: 30px 75px;
    }

    .footer__phone {
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        grid-column-start: 1;
        grid-column-end: span 2;
        grid-row-start: 1;
        grid-row-end: 1;
    }

    .footer__links {
        grid-column-start: 1;
        grid-row-start: 2;
    }

    .footer__social {
        justify-self: flex-end;
        margin-right: 37px;
        grid-column-start: 2;
        grid-row-start: 2;
    }
}

@media screen and (width <= 577px) {
    .footer {
        display: flex;
        flex-direction: column;
        align-items: center;
        max-width: 510px;
        height: 273px;
    }

    .footer__phone {
        width: 100%;
        height: 50px;
        flex-direction: row;
        justify-content: space-between;
    }

    .footer__links {
        width: 100%;
        height: 113px;
    }

    .footer__spliter {
        display: block;
    }

    .footer__social {
        width: 176px;
        height: 48px;
        margin: 0;
    }

    .social__rights {
        display: flex;
        align-items: center;
        justify-content: center;
    }
}

@font-face {
    font-family: Raleway;
    src: url('/public/fonts/Raleway-VariableFont_wght.ttf');
}

</style>