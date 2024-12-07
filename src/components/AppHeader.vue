<template>
    <div class="app__header">
        <header class="header">
            <div class="header__logo container">
                <img src="house__logo.svg" alt="logo" class="header__logo picture">
            </div>
            <hr class="header_line_510">
            <div class="hamburger__menu">
                <button class="hamburger button" @click="hamburgerActive=!hamburgerActive"></button>
                <nav v-if="hamburgerActive" class="hamburger_navigation">
                    <button class="hamburger button" @click="hamburgerActive=!hamburgerActive"></button>
                    <RouterLink to="/">Репродукции</RouterLink>
                    <RouterLink to="/">Новинки</RouterLink>
                    <RouterLink to="/">О нас</RouterLink>
                </nav>
                <RouterLink to="/"><img src="cart.svg" alt="cart" class="navigation__cart picture"></RouterLink>
            </div>
            <nav class="header__navigation">
                <RouterLink to="/">Репродукции</RouterLink>
                <RouterLink to="/">Новинки</RouterLink>
                <RouterLink to="/">О нас</RouterLink>
                <RouterLink to="/"><img src="cart.svg" alt="cart" class="navigation__cart picture"></RouterLink>
            </nav>
        </header>
    </div>
</template>
<script>
export default {
    data() {
        return {
            hamburgerActive: false
        }
    },
}
</script>
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

.header__logo.container {
    width: 100%;
}

.header__logo.picture {
    width: 143px;
    height: 35px;
}

.header_line_510 {
    display: none;
    width: 510px;
    background-color: #C3D1C6;
}

.hamburger__menu {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 15px;
    width: 290px;
    height: 62px;
}

.hamburger.button {
    width: 30px;
    height: 30px;
    margin: 0;
    background-image: url("/public/hamburger.svg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
    border: none;
    background-color: transparent;
}

.hamburger__icon {
    width: 24px;
    height: 24px;
}

.hamburger_navigation {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    position: absolute;
    width: 288px;
    height: 433px;
    background-color: #E1EDE6;
    padding: 16px 15px;
    transform: translate(-15px, 202px);
}

.hamburger_navigation a {
    text-decoration: none;
    color: #2C2D35;
    font-family: Raleway;
    font-size: 18px;
    font-weight: 500;
    line-height: 21.13px;
    text-align: left;
    margin: 30px 0 20px 0;
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

.navigation__cart.picture {
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

    .navigation__cart.picture {
        margin-left: 64px;
    }

    .header_line_510 {
        display: block;
    }
}

@media screen and (width <= 321px) {
    .header {
        padding: 0;
        height: 130px;
    }

    .header__logo.container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 68px;
        background-color: #FFFFFF;
    }

    .header_line_510 {
        display: none;
    }

    .header__navigation {
        display: none;
    }
}

@font-face {
    font-family: Raleway;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>