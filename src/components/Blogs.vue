<template>
    <div class="blogs" id="blogs">
        <div class="container">
            <div class="section-heading">
                <h1>Blog Posts</h1>
                <ul>
                    <li v-for="blog in blogs" v-bind:key=blog.id><a v-bind:href="blog.link">{{ blog.title }}</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            blogs: [
                { id: 1, title: 'Enumeration in Ruby', link: 'https://dev.to/eidorianavi/enumeration-in-ruby-2ooi'},
                { id: 2, title: 'Functions and the Single Responsibility Principle', link: 'https://dev.to/eidorianavi/functions-and-the-single-responsibility-principle-48ae'},
                { id: 3, title: 'querySelector vs. getElementById', link: 'https://dev.to/eidorianavi/queryselector-vs-getelementbyid-gm1'},
                { id: 4, title: 'Modular JavaScript: An Inrto to Import and Export', link: 'https://dev.to/eidorianavi/modular-javascript-an-intro-to-import-and-export-2khi'},
                { id: 5, title: 'My time at a coding bootcamp', link: 'https://medium.com/@reneavila1993/my-time-at-a-coding-boot-camp-40238c7a8b0c'},
            ]
        }
    }
}
</script>

<style>
.blogs {
    height: 100vh;
    width: 100%;
}
</style>