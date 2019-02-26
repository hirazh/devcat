<template>
    <div class="layout-container">  
        <Nav />
        <component :is="layout"></component>
    </div>
</template>

<script>

import BlogPostList from './BlogPostList.vue'
import PostView from './PostView.vue'
import Nav from './components/Nav.vue'
import Header from './components/Header.vue'

export default {
    name: 'layout',
    components: {
        BlogPostList,
        PostView,
        Nav,
        Header
    },
    computed: {
        layout() {
            return this.$page.frontmatter.layout
        }
    }
}
</script>

<style>
html {
    background-color: #17141D;
    color: #f0f0f0;
}
</style>
