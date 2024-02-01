<script>
export default {
    name: "AppFooterTop",
    data: () => ({
        dc_logo_bg: 'dc-logo-bg.png',
    }),
    methods: {
        createImagePath(image) {
            const url = new URL(`../../assets/img/${image}`,
                import.meta.url);
            return url.href;
        }
    }
};
</script>

<template>
    <div class="footer-top">
        <nav class="footer-row">
            <div class="footer-col">
                <h4>DC COMICS</h4>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Video</a></li>
                    <li><a href="#">News</a></li>
                </ul>

                <h4>SHOP</h4>
                <ul>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibibles</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>DC</h4>
                <ul>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy policy(New)</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>SITES</h4>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </div>
            <figure>
                <img :src="createImagePath(dc_logo_bg)" alt="dc-logo-bg">
            </figure>
        </nav>
    </div>
</template>

<style lang="scss" scoped>
.footer-top {
    height: 430px;
    background-image: url(../../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}


.footer-row {
    display: flex;
    max-width: 1400px;
    margin: 0 auto;
    position: relative;
}

.footer-col {
    flex-basis: calc(40% / 3);

    li {
        list-style-type: none;
    }

    a {
        text-decoration: none;
        color: rgba(211, 211, 211, 0.783);
        font-size: 0.8rem;
    }

    h4 {
        color: white;
        margin: 20px 0;
    }
}


img {
    height: 430px;
    position: absolute;
    right: 0;
}
</style>