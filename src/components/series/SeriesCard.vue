<script>
export default {
    name: "SeriesCard",
    props: {
        image: String,
        title: String
    }
};
</script>

<template>
    <div class="series-card">
        <img :src="image" :alt="title">
        <h3>{{ title }}</h3>
    </div>
</template>

<style lang="scss" scoped>
.series-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 10px;

    img {
        width: 100px;
        height: 100px;
        display: block;
    }

    h3 {
        padding-top: 5px;
        color: white;
        font-size: 0.8rem;
    }
}
</style>