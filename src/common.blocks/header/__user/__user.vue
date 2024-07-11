<template>
    <div class="__user">
        <img class="__user-ico" 
            src="./__user.svg" 
            alt="Логотип" 
            draggable="false"
        >
        <p class="__user-mailbox"
        > {{ userMailbox }}
        </p>
    </div>
</template>

<script>
export default {
    name: 'UserInfoView',
    data(){
        return {
            userMailbox: 'Username@adaurum.ru'
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "./__user"
</style>
