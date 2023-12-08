<script>
import AppTopFooterList from './AppTopFooterList.vue';

export default {
    data() {
        return {

        }
    },
    components: {
        AppTopFooterList
    }

}
</script>

<template>
    <div class="top-footer">
        <div class="wrapper">
            <AppTopFooterList />
        </div>
    </div>
</template>

<style lang="scss" scoped>
.top-footer {
    background-image: url(../../public/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .wrapper {
        justify-content: flex-start;
        align-items: flex-start;
        gap: 30px;
    }
}
</style>
