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
        <a href="#"><img :src="img" :alt="title"></a>
    </div>
    <a class="comic-title" href="#">
        <h5>{{ title }}</h5>
    </a>
</template>

<style lang="scss" scoped>
.pic-container {
    width: 100%;
    aspect-ratio: 1 / 1;
    overflow: hidden;
}

.comic-title {

    h5 {
        color: white;
        font-family: 'Open Sans', sans-serif;
        text-transform: uppercase;
        font-weight: 400;
        margin-top: 20px;
    }

}
</style>