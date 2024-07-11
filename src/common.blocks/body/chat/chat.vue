<template>
    <div class="chat">
        <div class="chat-header__wrapper">
            <h1 class="text"> 
                Личный помощник 
            </h1>
            <p class="name">  
                {{ administratorName }}
            </p>
            <p class="mailBox">  
                {{ administratorMailbox }}
            </p>
            <ChatFeedbackView class="chat_feedback"/>
        </div>

        <ChatEmptyView class="chat_empty"/>
        <GalleryButtonView class="chat_gallery"/>
        <AddFolderView class="chat_add-folder"/>
        <EnterButtonView class="chat_enter"/>
    </div>
</template>

<script>
import ChatEmptyView from "./chat_empty/chat_empty.vue"
import ChatFeedbackView from "./chat-feedback/chat-feedback.vue"
import GalleryButtonView from "./gallery-button/gallery-button.vue"
import AddFolderView from "./add-folder/add-folder.vue"
import EnterButtonView from "./enter-button/enter-button.vue"
export default {
    name: 'ChatView',
    data() {
        return {
            administratorName: 'Jim Davidson',
            administratorMailbox: 'JimDavidson@adaurum.ru'
        }
    },
    components:{
        ChatEmptyView,
        ChatFeedbackView,
        GalleryButtonView,
        AddFolderView,
        EnterButtonView
    }
}
</script>

<style lang="scss" scoped>
    @import "./chat"
</style>
