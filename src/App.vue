<template>
  <AppHeader />
  <router-view/>
  <AppFooter />
</template>

<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';

export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
</style>
