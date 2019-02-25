<template>
    <div class="bloglist-container">
        <Header />
        <router-link class="router-link" v-for="post in posts" :to="post.path">
            <h1>{{post.frontmatter.title}}</h1>
        </router-link>
        <Content />
    </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
    name: 'BlogPostList',
    components: { Header },
    computed: {
        posts() {
            return this.$site.pages
            .filter(x => x.path.startsWith('/blogs/'))
        }
    }
}
</script>

<style scoped>

.router-link {
    color: black;
    text-decoration-line: none;
}

</style>
