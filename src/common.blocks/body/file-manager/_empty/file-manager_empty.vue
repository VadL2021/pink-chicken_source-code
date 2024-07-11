<template>
    <div class="file-manager_empty">
        <h1 class="label">
            Файлы
        </h1>
        <img class="image"
            src="./file-manager_empty.svg" 
            alt="Картинка на фоне пустого каталога файлов"
            draggable="false"
        >
        <p class="text">
            Закажи у личного помощника медиаплан. Он появится в этом разделе
        </p>
    </div>
</template>

<script>
export default {
    name: 'FileManagerEmptyView'
}
</script>

<style lang="scss" scoped>
    @import "./file-manager_empty"
</style>
