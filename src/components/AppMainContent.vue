<script>
export default {
    name: "AppMainContent",
};
</script>

<template>
    <main>
        <div class="content-container">
            <h2>Content Goes here</h2>
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #1C1C1C;
}

.content-container {
    height: 100px;
    max-width: 1400px;
    margin: 0 auto;
    display: flex;
    align-items: center;

    h2 {
        color: white;
    }
}
</style>