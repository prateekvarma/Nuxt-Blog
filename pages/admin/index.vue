<template>
    <div>
        <section>
            <button @click="$router.push('/admin/new-post')">Create Post</button>
        </section>
        <section>
            <h1>Existing Posts</h1>
            <post-list />
        </section>
    </div>
</template>

<script>
import PostList from '~/components/Posts/PostList.vue'

export default {
    components: {
        PostList
    }
}
</script>