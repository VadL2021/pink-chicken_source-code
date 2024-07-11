<template>
    <button class="enter-button">
        <img class="image"
            src="./enter-button.svg" 
            alt="Картинка на фоне пустого каталога файлов"
            draggable="false"
        >
        <p class="enter-text">Enter</p>
    </button>

</template>

<script>
export default {
    name: 'EnterButtonView'
}
</script>

<style lang="scss" scoped>
    @import "./enter-button"
</style>
