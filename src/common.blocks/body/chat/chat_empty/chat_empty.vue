<template>
    <div class="chat_empty">
        <img class="image"  
            src="./chat_empty.svg" 
            alt="Картинка с образом администратора"
            draggable="false"   
        >
        <p class="text">
            Это чат с администратором. 
            Ты можешь с ним пообщаться по любому вопросу 
            о нашем сервисе и узнать о ходе работы
        </p>
        <textarea class="chat-input" 
            placeholder="Введите сообщение для администратора"
            rows="8"
            maxlength="260"
        ></textarea>
        <button @click="this.$store.state.MediaPlanIsRequisted = true" class="mediaplan-button">
            Заказать медиаплан
        </button>
        <button @click="this.$store.state.ReportIsRequisted = true" class="report-button">
            Заказать отчет
        </button>
    </div>
</template>

<script>
export default {
    name: 'ChatEmptyView',
    data() {
        return {
            administratorName: 'Jim Davidson',
            administratorMailbox: 'JimDavidson@adaurum.ru'
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "./chat_empty"
</style>
