<template>
    <div class="picture__card">
        <img :src="pictureData.url" :alt="pictureData.pictureName">
        <p>{{ pictureData.author }}</p>
        <h3>{{ pictureData.pictureName }}</h3>
        <p>{{ pictureData.style }} {{ pictureData.size }}</p>
        <p> {{ pictureData.price }}</p>
        <button>В корзину</button>
    </div>
</template>

<script>
export default {
    props: {
        pictureData: Object
    }
}
</script>