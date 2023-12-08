<script>


export default {
    data() {
        return {

        }
    },

}
</script>

<template>
    <button>Sign-up now!</button>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

button {
    text-transform: uppercase;
    background-color: transparent;
    border: 2px solid $main-color;
    color: white;
    font-weight: bold;
    padding: 15px;
    margin: 30px 0
}
</style>
