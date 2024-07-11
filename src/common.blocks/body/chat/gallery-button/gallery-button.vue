<template>
    <button class="gallery-button">
        <img class="image"
            src="./gallery-button.svg" 
            alt="Кнопка открывающая галлерею"
            draggable="false"
        >
    </button>
</template>

<script>
export default {
    name: 'GalleryButtonView'
}
</script>

<style lang="scss" scoped>
    @import "./gallery-button"
</style>
