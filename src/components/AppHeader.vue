<template>
    <div class="app__header">
        <header class="header">
            <img src="house__logo.svg" alt="logo" class="header__logo">
            <hr class="header_line_510">
            <nav class="header__navigation">
                <RouterLink to="/">Репродукции</RouterLink>
                <RouterLink to="/">Новинки</RouterLink>
                <RouterLink to="/">О нас</RouterLink>
                <RouterLink to="/"><img src="cart.svg" alt="cart" class="navigation__cart"></RouterLink>
            </nav>
        </header>
    </div>
</template>
<style>
.app__header {
    background-color: #E1EDE6;
    margin: 0;
}

.header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 0 auto;
    max-width: 1110px;
    height: 100px;
    padding: 0 15px;
}

.header__logo {
    width: 143px;
    height: 35px;
}

.header_line_510 {
    display: none;
    width: 510px;
    background-color: #C3D1C6;
}

.header__navigation {
    display: flex;
    align-items: center;
    gap: 60px;
    font-family: Raleway;
}

.header__navigation a {
    text-decoration: none;
    color: #2C2D35;
    font-family: Raleway;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    text-align: left;
}

.navigation__cart {
    width: 24px;
    height: 24px;
}

@media screen and (width <= 769px) {
    .header__navigation a {
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }
}

@media screen and (width <= 577px) {
    .header {
        flex-direction: column;
        height: 91px;
        padding: 16px 33px;
    }

    .header_line_510 {
        display: block;
    }
}

@font-face {
    font-family: Raleway;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>