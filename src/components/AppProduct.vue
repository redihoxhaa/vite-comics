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

<style lang="scss" scoped></style>