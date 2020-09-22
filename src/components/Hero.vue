<template>
    <div class="banner-page">
        <div class="banner-text">
            <h1>Adrian Avila</h1>
            <h6>Full Stack Software Engineer</h6>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.banner-page {
    width: 100%;
    height: 100vh;
}

.banner-text {
    font-family: 'Permanent Marker', cursive;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate( -50%, -50%);
    width: 100%;
    text-align: center;
    user-select: none;
}

h1 {
    font-size: 13rem;
}

h6 { 
    font-size: 2rem;
    font-weight: 300;
}
</style>