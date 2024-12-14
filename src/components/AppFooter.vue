<template>
    <div class="app__footer">
        <div class="footer">
            <div class="footer__phone"></div>
            <div class="footer__links"></div>
            <div class="footer__social"></div>
        </div>
    </div>
</template>

<style>
.app__footer {
    width: 100%;
    height: 168px;
    background-color: #E1EDE6;
}

.footer {
    width: 1110px;
    height: 100%;
    margin: 0 auto;
    align-items: flex-start;
    justify-content: center;
    align-content: center;
    display: grid;
    grid-template-columns: 170px 445px 132px;
}

.footer__phone {
    width: 170px;
    height: 122px;
    background-color: purple;
}

.footer__links {
    width: 445px;
    height: 122px;
    background-color: blue;
}

.footer__social {
    justify-self: flex-end;
    width: 132px;
    height: 68px;
    background-color: red;
}

@media screen and (width <= 769px) {
    .footer {
        grid-template-columns: 445px 170px;
    }

    .footer__phone {
        grid-column-start: 1;
        grid-column-end: 2;
        grid-row-start: 1;
        grid-row-end: 1;
    }

    .footer__links {
        grid-column-start: 1;
        grid-column-end: 1;
        grid-row-start: 2;
        grid-row-end: 2;
    }

    .footer__social {
        grid-column-start: 2;
        grid-column-end: 2;
        grid-row-start: 2;
        grid-row-end: 2;
    }
}
</style>