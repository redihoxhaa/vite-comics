<script>
export default {}
</script>

<template>
    <div class="jumbotron">
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;

.jumbotron {
    height: 400px;
    @include background-placer('../../../public/img/jumbotron.jpg', cover, top, no-repeat);
}
</style>