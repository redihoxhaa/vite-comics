<script>
export default {

    data() {
        return {
            blueBarElements: [
                {
                    text: 'digital comics',
                    img: '../../public/img/buy-comics-digital-comics.png',
                },
                {
                    text: 'dc merchandise',
                    img: '../../public/img/buy-comics-merchandise.png',
                },
                {
                    text: 'subscription',
                    img: '../../public/img/buy-comics-subscriptions.png',
                },
                {
                    text: 'comic shop locator',
                    img: '../../public/img/buy-comics-shop-locator.png',
                },
                {
                    text: 'dc power visa',
                    img: '../../public/img/buy-dc-power-visa.svg',
                },
            ]

        }
    }
}
</script>

<template>
    <ul>
        <li v-for="element in blueBarElements">
            <div class="pic-container">
                <img :src="element.img" :alt="element.text">
            </div>
            <span>{{ element.text }}</span>
        </li>
    </ul>
</template>

<style scoped lang="scss">
ul {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 80px;

    li {
        display: flex;
        justify-content: center;
        align-items: center;

        .pic-container {
            width: 50px;
            height: 50px;
        }

        span {
            color: white;
            text-transform: uppercase;
        }
    }
}
</style>
