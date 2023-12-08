<script>


export default {
    data() {
        return {
            linksList: [
                {
                    listTitle: 'DC Comics',
                    listElements: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                },
                {
                    listTitle: 'Shop',
                    listElements: ['Shop DC', 'Shop DC Collectibles']
                },
                {
                    listTitle: 'DC',
                    listElements: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices ', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                },
                {
                    listTitle: 'Sites',
                    listElements: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                },
            ]
        }
    },

}
</script>

<template>
    <div class="col">
        <ul>
            <li>{{ linksList[0].listTitle }}</li>
            <li v-for="element in linksList[0].listElements"><a href="#">{{ element }}</a></li>
        </ul>
        <ul>
            <li>{{ linksList[1].listTitle }}</li>
            <li v-for="element in linksList[1].listElements"><a href="#">{{ element }}</a></li>
        </ul>
    </div>

    <div class="col">
        <ul>
            <li>{{ linksList[2].listTitle }}</li>
            <li v-for="element in linksList[2].listElements"><a href="#">{{ element }}</a></li>
        </ul>
    </div>

    <div class="col">
        <ul>
            <li>{{ linksList[3].listTitle }}</li>
            <li v-for="element in linksList[3].listElements"><a href="#">{{ element }}</a></li>
        </ul>
    </div>

    <!-- Modo per ciclare le liste, però senza la possibilità di mettere due liste nella stessa colonna
    <div class="col" v-for="lists in linksList">
        <ul>
            <li>{{ lists.listTitle }}</li>
            <li v-for="element in lists.listElements"> {{ element }}</li>
        </ul>
    </div>
     -->
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.col {
    display: flex;
    flex-direction: column;
    gap: 30px;
    padding: 60px 0;

    ul {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        gap: 6px;


        li {
            font-size: 14px;
            font-family: 'Open Sans', sans-serif;
            font-weight: 500;
            color: $light-gray;

            &:first-child {
                font-family: 'Asap Condensed', sans-serif;
                text-transform: uppercase;
                font-weight: bold;
                font-size: 1.5rem;
                margin-bottom: 10px;
                color: white;
            }
        }
    }
}
</style>
