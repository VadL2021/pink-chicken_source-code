<template>
    <div class="file-manager">
        <!-- //Я понимаю какой это костыль
            //я просто не успеваю сделать лучше
            //прошу не судить строго -->
        <FileManagerEmptyView 
            v-if="!this.$store.state.MediaPlanIsRequisted && 
            !this.$store.state.ReportIsRequisted" 
            class="file-manager_empty" />
        <FileManagerFilledView 
            v-if="this.$store.state.MediaPlanIsRequisted || 
            this.$store.state.ReportIsRequisted"
            class="file-manager_filled" /> 
    </div>
</template>

<script>
import FileManagerEmptyView from "./_empty/file-manager_empty.vue"
import FileManagerFilledView from "./_filled/file-manager_filled.vue"
export default {
    name: 'FileManagerView',
    components:{
        FileManagerEmptyView,
        FileManagerFilledView
    }
}
</script>

<style lang="scss" scoped>
    @import "./file-manager"
</style>
