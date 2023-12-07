<script>
import AppHeader from './components/AppHeader.vue';
import AppBlueBar from './components/AppBlueBar.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  data() {
    return {

    }
  },
  components: {
    AppHeader,
    AppBlueBar,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppBlueBar />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
