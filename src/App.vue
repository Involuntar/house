<template>
  <AppHeader />
  <router-view/>
  <AppFooter class="AppFooter"/>
  <AppFooterMobile class="AppFooterMobile" />
</template>

<script>
import AppFooter from './components/AppFooter.vue';
import AppFooterMobile from './components/AppFooterMobile.vue';
import AppHeader from './components/AppHeader.vue';

export default {
  components: {
    AppHeader,
    AppFooter,
    AppFooterMobile
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

.AppFooterMobile {
  display: none;
}

@media screen and (width <= 376px) {
  .AppFooterMobile {
    display: block;
  }

  .AppFooter {
    display: none;
  }
}

</style>
