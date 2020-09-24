<template>
    <div class="portfolio" id="portfolio">
        <div class="container">
            <div class="section-heading">
                <h1>Portfolio</h1>
                <h6>Recent Work</h6>
            </div>
            <div class="demo-videos">
                <div class="portfolio-item">
                    <h2>smallTalk</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/aZMOCxSa3Yg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="portfolio-item">
                    <h2>theRack</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/5GngnwWPQiI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="portfolio-item">
                    <h2>Jedi Archives</h2>
                    <div class="iframe-container">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/XglSvmMSHPk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
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

.portfolio {
    margin-top: 20rem;
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 2rem;
}

.section-heading h1 {
    font-size: 10rem;
    opacity: .5;
}

.section-heading h6 { 
    font-size: 3rem;
    font-style: italic;
    font-weight: 300;
    margin-top: 3rem;
    opacity: .7;

}

.demo-videos {
    width: 10%;
    margin-top: 3rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.iframe-container{
    padding: 5rem;
    width: 80%;
    /* padding-bottom: 56.25%; */
}

.iframe-container iframe{
    margin-bottom: 2rem;
    top: 0;
    left: 0;
}


</style>