<script>
export default {}
</script>

<template>
    <button><a href="#">Load More</a></button>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

button {

    margin-bottom: 30px;

    a {
        color: white;
        text-transform: uppercase;
        padding: 10px 60px;
        background-color: $main-color;
        font-family: 'Asap Condensed', sans-serif;
        font-weight: bold;
        font-size: 1rem;
    }

}
</style>