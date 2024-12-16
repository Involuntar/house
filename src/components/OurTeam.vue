<template>
    <div class="team" id="team">
        <div class="team__pic">
            <img src="border.png" alt="border" class="team_pic_border">
            <img src="brushes.png" alt="brushes" class="team_pic_brushes">
        </div>
        <div class="team_about">
            <h1 class="team_about_header">Наша команда</h1>
            <p class="team_about_paragraph">
                Значимость этих проблем настолько очевидна, что базовый вектор развития
                позволяет оценить значение экспериментов, поражающих по своей масштабности и грандиозности. Мы вынуждены
                отталкиваться от того, что консультация с широким активом.
            </p>
            <div class="team_about_avatars">
                <img src="avatar1.png" alt="avatar1" class="team_about_avatar">
                <img src="avatar2.png" alt="avatar2" class="team_about_avatar">
                <img src="avatar3.png" alt="avatar3" class="team_about_avatar">
            </div>
        </div>
    </div>
</template>

<style>
.team {
    display: flex;
    align-items: center;
    max-width: 1110px;
    gap: 30px;
    padding: 79px 15px 0;
    margin: 70px auto 0;
}

.team__pic {
    position: relative;
    width: 445px;
    height: 361px;
}

.team_pic_border {
    width: 445px;
    height: 361px;
}

.team_pic_brushes {
    position: absolute;
    left: 48px;
    bottom: 43px;
    width: 269px;
    height: 397px;
}

.team_about {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    gap: 20px;
    font-family: Raleway;
}

.team_about_header {
    font-size: 40px;
    font-weight: 500;
    line-height: 44px;
    margin: 0 0 20px 0;
}

.team_about_paragraph {
    font-size: 18px;
    font-weight: 500;
    line-height: 27px;
}

.team_about_avatars {
    display: flex;
    align-items: center;
    gap: 30px;
}

.team_about_avatar {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    object-fit: cover;
    object-position: center;
}

@media screen and (width <= 769px) {
    .team {
        max-width: 690px;
        flex-direction: column;
        align-items: flex-start;
        gap: 40px;
    }

    .team__pic, .team_pic_border {
        width: 510px;
        height: 413px;
    }

    .team_pic_brushes {
        width: 308px;
        height: 455px;
        left: 55px;
        bottom: 49px;
    }

    .team_about {
        gap: 30px;
    }
    
    .team_about_header {
        font-size: 30px;
        font-weight: 500;
        line-height: 33px;
        margin: 0;
    }

    .team_about_paragraph {
        font-size: 18px;
        font-weight: 500;
        line-height: 27px;
        margin: 0;
    }
}

@media screen and (width <= 577px) {
    .team {
        max-width: 510px;
        gap: 30px;
    }

    .team__pic, .team_pic_border {
        width: 375px;
        height: 304px;
    }

    .team_pic_brushes {
        width: 227px;
        height: 334px;
        left: 40px;
        bottom: 36px;
    }

    .team_about {
        gap: 20px;
    }
    
    .team_about_header {
        font-size: 24px;
        font-weight: 500;
        line-height: 26.4px;
    }

    .team_about_paragraph {
        font-size: 16px;
        font-weight: 500;
        line-height: 22.4px;
    }
}

@media screen and (width <= 376px) {
    .team {
        max-width: 290px;
    }

    .team__pic, .team_pic_border {
        width: 290px;
        height: 235px;
    }

    .team_pic_brushes {
        width: 175px;
        height: 258px;
        left: 31px;
        bottom: 28px;
    }
    
    .team_about_header {
        font-size: 24px;
        font-weight: 500;
        line-height: 26.4px;
    }

    .team_about_paragraph {
        font-size: 16px;
        font-weight: 500;
        line-height: 22.4px;
    }
}

@font-face {
    font-family: RaleWay;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>