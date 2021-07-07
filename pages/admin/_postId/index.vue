<template>
    <div>
        <admin-post-form />
    </div>
</template>

<script>
import AdminPostForm from '~/components/Admin/AdminPostForm.vue'
export default {
    components: {
        AdminPostForm
    },
    data() {
        return {
            loadedPost: {
                author: 'Prateek',
                title: 'The title',
                content: 'This is the content',
                thumbnailLink: 'https://picture.jpeg'
            }
        }
    }
}
</script>