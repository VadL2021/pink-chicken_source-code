<template>
  <HeaderView class="header" />
  <BodyView class="body" />
  <FooterView class="page-footer" />
</template>

<script>
import HeaderView from './common.blocks/header/header.vue'
import BodyView from './common.blocks/body/body.vue'
import FooterView from './common.blocks/footer/footer.vue'

export default {
  name: 'App',
  components: {
    HeaderView,
    BodyView,
    FooterView
  }
}
</script>

<style>
  *{
    position: relative;
    margin:0;
    border-width: 0;
  }
  :root{
    height: 100%;
    background-color: #F5F5F5;
  }
</style>
