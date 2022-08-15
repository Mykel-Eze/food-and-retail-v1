<template>
    <div id="main-wrapper">
        <section class="error-container">
            <div class="row">
                <div class="container">
                    <div class="error-block center">
                        <img src="../assets/images/coming-soon.svg" alt="coming soon" class="coming-soon-img">
                        <div class="error-action-btn-wrapper">
                            <router-link to="/" custom v-slot="{ navigate }">
                                <button class="error-action-btn hover-scale" @click="navigate" role="link">
                                    Take me back home
                                    <img src="../assets/images/right-chevron.svg" alt="right" class="right-chevron">
                                </button>
                            </router-link>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: "ComingSoon"
}
</script>

<style scoped>
.error-block {
    padding: 15px;
}
h1.error-page-title {
    letter-spacing: -1px;
}
img.coming-soon-img {
    margin: 20px 0;
}
p.error-description {
    font-size: 18px;
    line-height: 19px;
    text-align: center;
    color: #6E7883;
}
.error-action-btn-wrapper {
    margin: 30px 0;
}
button.error-action-btn {
    background: #25A9E0;
    border-radius: 8px;
    border: none;
    font-weight: 500;
    font-size: 14px;
    line-height: 18px;
    color: white;
    height: 50px;
    width: 220px;
    cursor: pointer;
}
@media(min-height: 960px) {
    .error-container {
        min-height: 50vh;
    }
    .error-block {
        position: relative;
        top: 7vh;
    }
}
</style>