<template>
    <div class="dashboard">
        <img class="dashboard__ico.svg" src="./__ico.svg" 
            alt="Иконка документа xml в левой части дашборда"
        >
        <p class="dashboard__company-name">{{ companyName }}</p>
            <img class="dashboard__download-button-ico" 
                src="./__download-button.svg" 
                alt="Кнопка загрузки"
            > 
        <img v-if="!isLoaded" class="dashboard__loading-ico" 
         src="./__loading-ico.svg" 
            alt="Иконка документа xml в левой части дашборда"
        >
    </div>
</template>

<script>
export default {
    name: 'DahshboardView',
    props:{
        companyName: {
            type: String,
            requared: true
        },
        isLoaded: {
            type: Boolean,
            requared: true
        },
    }
}
</script>

<style lang="scss" scoped>
    @import "./dashboard"
</style>
