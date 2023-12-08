<script>


export default {
    data() {
        return {

        }
    },

}
</script>

<template>
    <button><a href="#">Sign-up now!</a></button>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

button {
    text-transform: uppercase;
    background-color: transparent;
    border: 2px solid $main-color;
    color: white;
    padding: 15px;
    margin: 30px 0;
    font-size: 1.125rem;
}
</style>
