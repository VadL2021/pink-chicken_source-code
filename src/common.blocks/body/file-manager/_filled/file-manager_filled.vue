<template>
    <div class="file-manager_filled">
        <h1 class="label">
            Файлы
        </h1>
        <h2 v-if="this.$store.state.MediaPlanIsRequisted" 
            class="label-media">
            Медиапланы
        </h2>
        <div class="content-wrapper">
        <ul v-if="this.$store.state.MediaPlanIsRequisted" 
            style="list-style-type: none; right:18px;">
            <li v-for="item in companyNamesA" :key="item.id">
                <DahshboardView :companyName="item" :isLoaded = true />
            </li>
        </ul>
        <h2 v-if="this.$store.state.ReportIsRequisted" 
            class="label-report">
            Отчеты
        </h2>
        <ul v-if="this.$store.state.ReportIsRequisted" style="list-style-type: none; right:18px;">
            <li v-for="item in companyNamesB" :key="item.id">
                <DahshboardView :companyName="item" :isLoaded = true />
            </li>
        </ul>
        </div>
    </div>
</template>

<script>
import DahshboardView from "./dashboard/dashboard.vue"
export default {
    name: 'FileManagerEmptyView',
    components: { 
        DahshboardView
    },
    data(){
        return{
            companyNamesA: [ 'Appify', 'Appstar', 'Apporddvas'],
            companyNamesB: [  'Appnova', 'Appzone', 'Appix']
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "./file-manager_filled"
</style>
