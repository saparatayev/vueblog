<template>
    <div>
        <div>
            <Article />
            <Article />
            <Article />
            <Article />
            <Article />
        </div>
        <div>
            <router-link to="/articles">View all</router-link>
        </div>
    </div>
</template>

<script>
import Article from './Article.vue'

export default {
    components: {
        Article
    },
    setup() {

    },
}
</script>
