<script>
import SeriesCard from './series/SeriesCard.vue'
export default {
    name: "AppMainContent",
    props: {
        series: Array
    },
    components: {
        SeriesCard
    }

};
</script>

<template>
    <main>
        <div class="position-button">
            <a role="button" href="#">CURRENT SERIES</a>
        </div>
        <div class="content-container">
            <SeriesCard v-for="(serie, i) in series" :key="i" :image="serie.thumb" :title="serie.title" />
        </div>
        <div class="button-container">
            <a role="button" href="#">LOAD MORE</a>
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #1C1C1C;
    position: relative;
}

.content-container {
    max-width: 1400px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    align-items: start;
    padding-top: 25px;

    .series-card {
        flex-basis: calc(100% / 6);
    }

    h2 {
        color: white;
    }
}

.button-container {
    padding: 20px 0;
    text-align: center;

    a {
        text-decoration: none;
        color: white;
        padding: 5px 40px;
        background-color: #0282F9;
        font-size: 0.8rem;
    }
}

.position-button {
    position: absolute;
    top: -12px;
    left: 15%;

    a {
        text-decoration: none;
        color: white;
        padding: 5px 10px;
        background-color: #0282F9;
        font-size: 1.1rem;
    }
}
</style>