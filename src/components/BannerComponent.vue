<template>
    <section>
        <img :src="bannerDetails.img" :alt="bannerDetails.title">
    
        <h2>{{ bannerDetails.title }}</h2>
    </section>
</template>

<script>
export default {
    name: "BannerComponent",
    props: {
        bannerDetails: Object
    }
}
</script>

<style lang="scss" scoped>
section {
    position: relative;
    height: 500px;

    img {
        height: 100%;
        object-fit: cover;
    }

    h2 {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: red;
        font-size: 50px;
    }
}
</style>