<template>
    <div class="picture__card">
        <img class="card__image" :src="pictureData.url" :alt="pictureData.pictureName">
        <div class="card__description">
            <p class="card__author">{{ pictureData.author }}</p>
            <h3 class="card__name">{{ pictureData.pictureName }}</h3>
            <p class="card__style">{{ pictureData.style }} ({{ pictureData.size }})</p>
            <p class="card__price"> {{ pictureData.price }}</p>
            <button class="card__cart button">В корзину</button>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        pictureData: Object
    }
}
</script>

<style>
.picture__card {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 350px;
    height: 680px;
    background-color: #E1EDE6;
    padding: 20px 0 30px;
    gap: 20px;
}

.card__description {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    width: 310px;
}

.card__image {
    width: 310px;
    height: 422px;
    object-fit: cover;
    object-position: center;
}

.card__author {
    margin: 0 0 10px;
    font-family: Raleway;
    font-size: 18px;
    font-weight: 500;
    line-height: 21.13px;
    color: #86928B;
}

.card__name {
    margin: 0 0 8px;
    font-family: Raleway;
    font-size: 30px;
    font-weight: 500;
    line-height: 35.22px;
    color: #2C2D35;
}

.card__style {
    margin: 0 0 30px;
    font-family: Raleway;
    font-size: 18px;
    font-weight: 500;
    line-height: 21.13px;
    color: #2C2D35;
}

.card__price {
    margin: 0 0 20px;
    font-family: Raleway;
    font-size: 24px;
    font-weight: 500;
    line-height: 28.18px;
    color: #598D66;
}

.card__cart.button {
    width: 310px;
    height: 65px;
    border: 1px solid #598D66;
    background-color: transparent;
    font-family: Raleway;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    padding: 21px 0;
    color: #598D66;
    cursor: pointer;
}

.card__cart.button:hover {
    background-color: #598D66;
    color: #F4F6F5;
}

.card__cart.button:active {
    background-color: #376B44;
    columns: #FFF;
}

@media screen and (width <= 1025px) {
    .picture__card {
        width: 330px;
    }
}

@media screen and (width <= 577px) {
    .picture__card {
        width: 240px;
        height: 464px;
    }

    .card__image {
        width: 200px;
        height: 250px;
    }

    .card__description {
        width: 200px;
    }

    .card__author {
        font-size: 16px;
        font-weight: 500;
        line-height: 18.78px;
    }

    .card__name {
        margin: 0 0 10px;
        font-size: 24px;
        font-weight: 500;
        line-height: 28.18px;
    }

    .card__style {
        font-size: 16px;
        font-weight: 500;
        line-height: 18.78px;
    }

    .card__price {
        margin: 0 0 10px;
        font-size: 20px;
        font-weight: 500;
        line-height: 23.48px;
    }

    .card__cart.button {
        width: 200px;
        height: 50px;
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
        padding: 14.5px 0;
    }
}

@media screen and (width <= 426px) {
    .picture__card {
        width: 290px;
        height: 464px;
    }

    .card__image {
        width: 250px;
        height: 250px;
    }

    .card__description {
        width: 250px;
    }

    .card__author {
        font-size: 16px;
        font-weight: 500;
        line-height: 18.78px;
    }

    .card__name {
        font-size: 24px;
        font-weight: 500;
        line-height: 28.18px;
    }

    .card__style {
        font-size: 16px;
        font-weight: 500;
        line-height: 18.78px;
    }

    .card__price {
        font-size: 20px;
        font-weight: 500;
        line-height: 23.48px;
    }

    .card__cart.button {
        width: 250px;
        height: 50px;
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }
}


@font-face {
    font-family: Raleway;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>