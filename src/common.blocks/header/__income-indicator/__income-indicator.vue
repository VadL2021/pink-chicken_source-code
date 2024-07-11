<template>
    <div class="__income-indicator">
        <img class="__income-indicator-ico" 
            src="./__income-indicator.svg" 
            alt="Логотип"
            draggable="false"
        >
        <p class="__income-indicator-percentage"
        > {{ `${revenuePercentage} %` }}
        </p>
    </div>
</template>

<script>
export default {
    name: 'RevenueIndicatorView',
    data(){
        return {
            revenuePercentage: 5
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "./__income-indicator"
</style>
