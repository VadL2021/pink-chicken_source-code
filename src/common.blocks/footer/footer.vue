<template>
  <div class="footer">
    <div class="container">
      <div class="wrapper">
        <LogoView class="footer-logo"/>
        <PrivacyPolicyView class="footer-privacy-policy"/>
        <MailBoxView class="footer-mail-box"/>
        <LanguageSelectorView class="footer-language-selector"/>
        <SocialNetworksView class="footer-social-networks"/>
      </div>
    </div>
  </div>
</template>

<script>
import LogoView from  "./__logo/__logo.vue"
import PrivacyPolicyView from "./__privacy-policy/__privacy-policy.vue"
import MailBoxView from './__mailbox/__mailbox.vue'
import LanguageSelectorView from './__language-selector/__language-selector.vue'
import SocialNetworksView from './__social-networks/__social-networks.vue'
  export default {
    name: 'FooterView',
    components:{
      LogoView,
      PrivacyPolicyView,
      MailBoxView,
      LanguageSelectorView,
      SocialNetworksView
    }
  }
</script>

<style lang="scss" scoped>
  @import "./footer"
</style>
  