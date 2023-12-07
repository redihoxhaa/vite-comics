<script>
import AppLogo from './AppLogo.vue';
import AppPagesList from './AppPagesList.vue'

export default {
    data() {
        return {

        }
    },
    components: {
        AppLogo,
        AppPagesList
    }
}
</script>

<template>
    <header>
        <div class="wrapper">
            <AppLogo />
            <AppPagesList />
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/utilities.scss' as *;

.wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;

}
</style>
