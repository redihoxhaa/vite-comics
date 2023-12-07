<script>
import AppBlueBarList from './AppBlueBarList.vue'
export default {
    data() {
        return {

        }
    },
    components: {
        AppBlueBarList
    }
}
</script>

<template>
    <section class="blue-links">
        <div class="wrapper">
            <AppBlueBarList />

        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;

.blue-links {
    padding: 50px 0;
    background-color: $main-color;
}
</style>
