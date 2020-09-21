<template>
    <div class="blogs" id="blogs">
        <div class="container">
            <div class="section-heading">
                <h1>Blog Posts</h1>
                <ul>
                    <li v-for="blog in blogs" v-bind:key='{{ blog.id }}'><a href={{ blog.link }}>{{ blog.title }}</a></li>
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
                { id: 1, title: '', link: ''},
                { id: 2, title: '', link: ''},
                { id: 3, title: '', link: ''},
                { id: 4, title: '', link: ''},
                { id: 5, title: '', link: ''},
            ]
        }
    }
}
</script>

<style>

</style>