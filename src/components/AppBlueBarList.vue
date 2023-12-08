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
            <a href="#">
                <div class="pic-container">
                    <img :src="element.img" :alt="element.text">
                </div>
                <span>{{ element.text }}</span>
            </a>
        </li>
    </ul>
</template>

<style scoped lang="scss">
ul {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    width: 100%;

    a {
        display: flex;
        justify-content: center;
        align-items: center;

        .pic-container {
            width: 50px;
            height: 50px;
            margin-right: 15px;

            img {
                height: 100%;
                object-fit: contain;
            }
        }

        span {
            color: white;
            text-transform: uppercase;
            font-family: 'Open Sans', sans-serif;
            font-weight: 100;
        }
    }
}
</style>
