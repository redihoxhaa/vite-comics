<script>
export default {
    data() {
        return {
            socialElements: [
                {
                    name: 'facebook',
                    img: '/img/footer-facebook.png',
                },
                {
                    name: 'twitter',
                    img: '/img/footer-twitter.png',
                },
                {
                    name: 'youtube',
                    img: '/img/footer-youtube.png',
                },
                {
                    name: 'pinterest',
                    img: '/img/footer-pinterest.png',
                },
                {
                    name: 'periscope',
                    img: '/img/footer-periscope.png',
                },
            ]

        }
    },

}
</script>

<template>
    <ul>
        <li class="call-to-action">Follow Us</li>
        <li v-for="element in socialElements"><a href="#">
                <div class="pic-container"><img :src="element.img" :alt="element.name"></div>
            </a></li>
    </ul>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;

ul {
    display: flex;
    align-items: center;
    gap: 20px;

    .call-to-action {
        text-transform: uppercase;
        color: $main-color;
        font-weight: 600;
        font-size: 20px;
    }
}
</style>
