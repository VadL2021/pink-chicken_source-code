<template>
    <div class="__logo">
      <img class="__language-selector-image-ico"
        src="./__language-selector.svg" 
        alt="Логотип"
        draggable="false"
      >
      <img class="__language-selector-image-RU"
        src="./__language-selector-RU.svg" 
        alt="Логотип"
        draggable="false"
      >
      <img class="__language-selector-image-EN"
        src="./__language-selector-EN.svg" 
        alt="Логотип"
        draggable="false"
      >      
      <img class="__language-selector-image-TUR"
        src="./__language-selector-TUR.svg" 
        alt="Логотип"
        draggable="false"
      >
    </div>
</template>

<script>
export default {
  name: 'LanguageSelectorView'
}
</script>

<style lang="scss" scoped>
  @import "./__language-selector"
</style>

