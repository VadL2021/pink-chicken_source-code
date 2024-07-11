<template>
  <div class="body">
    <FileManagerView class="file-manager" />
    <ChatView  class="chat" />
  </div>
</template>

<script>
  import FileManagerView from "./file-manager/file-manager.vue"
  import ChatView from "./chat/chat.vue"
  export default {
    name: 'PageContentView',
    components:{
      FileManagerView,
      ChatView
    }
  }
</script>

<style lang="scss" scoped>
  @import "./body"
</style>
