<script>
import AppTopFooter from './AppTopFooter.vue';
import AppBottomFooter from './AppBottomFooter.vue';

export default {
    data() {
        return {

        }
    },
    components: {
        AppTopFooter,
        AppBottomFooter
    }
}
</script>

<template>
    <footer>
        <AppTopFooter />
        <AppBottomFooter />

    </footer>
</template>

<style scoped lang="scss"></style>
