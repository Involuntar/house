<template>
    <div class="team">
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

@font-face {
    font-family: RaleWay;
    src: url("/public/fonts/Raleway-VariableFont_wght.ttf");
}
</style>