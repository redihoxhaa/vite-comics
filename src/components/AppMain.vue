<script>

import AppProducts from './AppProducts.vue';
import AppMainTitle from './AppMainTitle.vue';
import AppJumbotron from './AppJumbotron.vue';
import AppBlueBar from './AppBlueBar.vue';
export default {
    components: { AppProducts, AppMainTitle, AppBlueBar, AppJumbotron, },
    data() {
        return {};
    },

}
</script>

<template>
    <main>
        <AppJumbotron />
        <div class="wrapper">
            <AppMainTitle />
            <AppProducts />
        </div>
        <AppBlueBar />
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

main {
    background-color: $products-bg;

    .wrapper {
        position: relative;
        justify-content: center;
    }

    span {
        font-size: 1.5rem;
        color: white;
        font-weight: bold
    }

    ;
}
</style>
