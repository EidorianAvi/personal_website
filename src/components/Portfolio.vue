<template>
    <div class="portfolio" id="portfolio">
        <div class="container">
            <div class="section-heading">
                <h1>Portfolio</h1>
                <h6>Recent Work</h6>
            </div>
            <div class="portfolio-item">
                <div class="iframe-container">
                    <iframe width="560" height="315" src="https://www.youtube.com/embed/aZMOCxSa3Yg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
            <div class="portfolio-item">
                <div class="iframe-container">
                    <iframe width="560" height="315" src="https://www.youtube.com/embed/5GngnwWPQiI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
            <div class="portfolio-item">
                <div class="iframe-container">
                    <iframe width="560" height="315" src="https://www.youtube.com/embed/XglSvmMSHPk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.iframe-container{
    position: relative;
    width: 100%;
    padding-bottom: 56.25%;
    height: 0;
}

.iframe-container iframe{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}
</style>