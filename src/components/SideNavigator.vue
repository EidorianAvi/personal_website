<template>
    <div class="sidebar">
        <div class="dot" id="title-dot">
            <li><span class="dot-text">Welcome</span></li>
        </div>
        <div class="dot" id="about-dot">
            <li><span class="dot-text">About Me</span></li>
        </div>
        <div class="dot" id="projects-dot">
            <li><span class="dot-text">Projects</span></li>
        </div>
        <div class="dot" id="blogs-dot">
            <li><span class="dot-text">Blogs</span></li>
        </div>
        <div class="dot" id="contact-dot">
            <li><span class="dot-text">Contact Me</span></li>
        </div>
    </div> 
</template>

<script>
export default {
    methods: {

    }
}
</script>

<style>

.sidebar {
    right: 1vw;
    position: fixed;
    right: -900px;
    top: 25vh;
    z-index: 1;
}
.dot li {
    margin-top: 1vh;
    cursor: pointer;
    font-size:  4vh;
    transition: 200ms;
    text-align: right;
    direction: rtl;
}
.dot li:hover {
    transition: 200ms;
    color: grey;
}
.dot-text {
    position: relative;
    left: 500px;
    transition: 400ms;
}
.dot li:hover .dot-text {
    left: 500px;
    transition: 400ms;
}
@media screen and (min-width: 720px) {	
    .sidebar {
        right: 1.5vw;
        position: fixed;
        top: 27vh;
        z-index: 1;
    }
    .dot li {
        margin-top: 3vh;
        cursor: pointer;
        font-size: 2.5vw;
        transition: 500ms;
        text-align: right;
        direction: rtl;
    }
    .dot li:hover {
        transition: 200ms;
        color: red;
    }
    .dot-text {
        position: relative;
        left: 500px;
        transition: 400ms;
    }
    .dot li:hover .dot-text {
        left: 0;
        transition: 600ms;
    }
}
</style>