<script>
export default {
    name: "AppHeader",
    data: () => ({
        contents,
        dc_logo: 'dc-logo.png',
    }),
    methods: {
        createImagePath(image) {
            const url = new URL(`../assets/img/${image}`,
                import.meta.url);
            return url.href;
        }
    }
};
</script>

<template>
    <header>
        <div class="header-container">
            <div class="figure-container">
                <img :src="createImagePath(dc_logo)" alt="logo">
            </div>
            <div class="categories">
                <ul>
                    <li v-for="(content, i) in contents" :key="i"><a :href="content.url">{{ content.text.toUpperCase()
                    }}</a></li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    margin: 20px 0;
    width: 100%;
}

.header-container {
    height: 100px;
    max-width: 1400px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;

    ul {
        display: flex;
        padding: 0;
    }

    li {
        list-style-type: none;
        font-weight: bold;
    }

    a {
        text-decoration: none;
        padding: 55px 10px;
        color: #56616C;
    }

    a:hover {
        border-bottom: 4px solid #0282F9;
    }
}

.categories {
    height: 100%;
    display: flex;
    align-items: center;
}

.figure-container {
    height: 100%;
    display: flex;
    align-items: center;
}
</style>