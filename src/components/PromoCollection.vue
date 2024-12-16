<template>
    <section class="promo" id="promo">
        <div class="promo_container">
            <div class="promo__header">
                <img src="Star 2.svg" alt="star" class="header_promo_pic">
                <h1 class="header_promo_text">Новая коллекция французских авторов</h1>
            </div>
            <p class="promo__paragraph first">
                Сложно сказать, почему акционеры крупнейших компаний призывают нас к новым
                свершениям, которые, в свою очередь, должны быть заблокированы в рамках своих собственных рациональных
                ограничений.
            </p>
            <p class="promo__paragraph second">
                Принимая во внимание показатели успешности, граница обучения кадров предопределяет высокую
                востребованность
                направлений прогрессивного развития.
            </p>
            <button class="promo__introduce button">Ознакомиться</button>
        </div>
    </section>
</template>

<style>
.promo {
    position: relative;
    width: 100%;
    background: linear-gradient(to right, #000, #00000000);
    color: #FFF;
    font-family: Raleway;
    margin-top: 70px;
}

.promo::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    background-image: url("/public/oldman.png");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    z-index: -1;
}

.promo_container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    max-width: 1110px;
    padding: 70px 0;
    margin: 0 auto;
}

.promo__header {
    display: flex;
    align-items: center;
    gap: 20px;
}

.header_promo_pic {
    width: 80px;
    height: 80px;
}

.header_promo_text {
    font-size: 40px;
    font-weight: 500;
    line-height: 40px;
    width: 421px;
}

.promo__paragraph {
    font-size: 18px;
    font-weight: 500;
    line-height: 27px;
    max-width: 540px;
}

.promo__paragraph.first {
    margin-top: 20px;
    margin-bottom: 20px;
}

.promo__introduce.button {
    width: 257px;
    height: 65px;
    background-color: #EEDB6D;
    font-family: Raleway;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    padding: 21px 0;
    margin-top: 60px;
    border: none;
}

@media screen and (width <= 769px) {
    .promo_container {
        max-width: 690px;
    }

    .header_promo_pic {
        width: 60px;
        height: 60px;
    }

    .header_promo_text {
        font-size: 30px;
        font-weight: 500;
        line-height: 30px;
        width: 370px;
    }

    .promo__paragraph {
        max-width: 690px;
        font-size: 18px;
        font-weight: 500;
        line-height: 27px;
    }

    .promo__paragraph.first {
        margin-top: 30px;
    }

    .promo__introduce.button {
        width: 210px;
        height: 60px;
        font-size: 20px;
        font-weight: 500;
        line-height: 23.48px;
        padding: 18.5px 0;
        margin-top: 30px;
    }
}

@media screen and (width <= 577px) {
    .promo_container {
        max-width: 510px;
        padding: 50px 0;
    }

    .header_promo_pic {
        width: 50px;
        height: 50px;
    }

    .header_promo_text {
        font-size: 24px;
        font-weight: 500;
        line-height: 24px;
        width: 261px;
    }

    .promo__paragraph {
        max-width: 510px;
        font-size: 16px;
        font-weight: 500;
        line-height: 22.4px;
    }

    .promo__paragraph.first {
        margin-top: 20px;
    }

    .promo__introduce.button {
        width: 190px;
        height: 50px;
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
        padding: 14.5px 0;
        margin-top: 20px;
    }
}

@media screen and (width <= 376px) {
    .promo_container {
        max-width: 290px;
    }

    .header_promo_text {
        font-size: 24px;
        font-weight: 500;
        line-height: 24px;
        width: 230px;
    }

    .promo__paragraph {
        max-width: 510px;
        font-size: 16px;
        font-weight: 500;
        line-height: 22.4px;
    }

    .promo__introduce.button {
        width: 290px;
        height: 50px;
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
        margin-top: 30px;
    }
}

@font-face {
    font-family: Raleway;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>