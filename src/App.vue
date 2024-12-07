<template>
  <AppHeader />
  <router-view/>
</template>

<script>
import AppHeader from './components/AppHeader.vue';

export default {
  components: {
    AppHeader
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
</style>
