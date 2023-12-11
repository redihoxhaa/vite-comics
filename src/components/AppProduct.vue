<script>
export default {
    props: {
        img: String,
        title: String,
    },
}
</script>

<template>
    <div class="pic-container">
        <img :src="img" :alt="title">
    </div>
    <h5>{{ title }}</h5>
</template>

<style lang="scss" scoped>
.pic-container {
    width: 100%;
    aspect-ratio: 1 / 1;
    overflow: hidden;
}

h5 {
    color: white;
    font-family: 'Open Sans', sans-serif;
    text-transform: uppercase;
    margin-top: 20px;
    font-weight: 400;


}
</style>