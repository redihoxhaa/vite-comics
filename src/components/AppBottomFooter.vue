<script>
import AppSignUpBtn from './AppSignUpBtn.vue';
import AppFollowUs from './AppFollowUs.vue';

export default {
    data() {
        return {

        }
    },
    components: {
        AppSignUpBtn,
        AppFollowUs
    }

}
</script>

<template>
    <div class="bottom-footer">
        <div class="wrapper">
            <AppSignUpBtn />
            <AppFollowUs />
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.bottom-footer {
    background-color: $dark-gray;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>
