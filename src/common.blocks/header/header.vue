<template>
  <div class="header">
    <LogoView class="header__logo"/>
    <IncomIndicatorView class="header__revenue"/>
    <UserView class="header__user"/>
    <SettingsButtonView class="header__settings"/>
    <LogoutButtonView class="header__logout-button"/>
  </div>
</template>

<script>
  import LogoView from "./__logo/__logo.vue"
  import IncomIndicatorView from "./__income-indicator/__income-indicator.vue"
  import UserView from "./__user/__user.vue"
  import SettingsButtonView from "./__settings-button/__settings-button.vue"
  import LogoutButtonView from "./__logout-button/__logout-button.vue"
  export default {
    name: 'HeaderView',
    components:{
      LogoView,
      IncomIndicatorView,
      UserView,
      SettingsButtonView,
      LogoutButtonView
    }
  }
</script>

<style lang="scss" scoped>
  @import "./header"
</style>
