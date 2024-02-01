<script>
export default {
    name: "AppFooterBottom",
};
</script>

<template>
    <div class="footer-bottom">
        <div class="content">
            <div class="left">
                <a role="button" href="#">SIGN-UP NOW!</a>
            </div>
            <div class="right">
                <ul>
                    <li>
                        <h3>FOLLOW US</h3>
                    </li>
                    <li><i class="fa-brands fa-facebook" style="color: #ffffff;"></i></li>
                    <li><i class="fa-brands fa-twitter" style="color: #ffffff;"></i></li>
                    <li><i class="fa-brands fa-youtube" style="color: #ffffff;"></i></li>
                    <li><i class="fa-brands fa-pinterest" style="color: #ffffff;"></i></li>
                    <li><i class="fa-solid fa-location-dot" style="color: #ffffff;"></i></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer-bottom {
    height: 130px;
    background-color: #303030;
}

.right ul {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
}

.right ul li {
    list-style-type: none;
}

.right i {
    font-size: 1.5rem;
}

h3 {
    color: #0282F9;
}

.content {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1400px;
    margin: 0 auto;
}

a {
    text-decoration: none;
    color: white;
    padding: 10px;
    border: 2px solid #0282F9;
}
</style>