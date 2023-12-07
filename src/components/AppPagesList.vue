<script>
export default {
    data() {
        return {
            listItems: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop'
            ]
        }
    }
}
</script>

<template>
    <ul>
        <li v-for="element in listItems"><a :href="`https://www.dc.com/${element}`">{{ element }}</a></li>
    </ul>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

ul {
    display: flex;
    list-style-type: none;
    text-transform: uppercase;
    gap: 35px;

    li {
        position: relative;

        &:hover {
            color: $main-color;

            &::before {
                content: '';
                width: 100%;
                height: 5px;
                background-color: $main-color;
                position: absolute;
                top: 50px;
                left: 0;
            }
        }
    }

}
</style>