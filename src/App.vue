<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBlueBar from './components/AppBlueBar.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  data() {
    return {

    }
  },
  components: {
    AppHeader,
    AppMain,
    AppBlueBar,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppBlueBar />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
