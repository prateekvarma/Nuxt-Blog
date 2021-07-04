<template>
    <div>
        <section>
            <form @submit.prevent="onSave">
                <app-control-input v-model="editedPost.author">Author Name</app-control-input>
                <app-control-input v-model="editedPost.title">Title</app-control-input>
                <app-control-input v-model="editedPost.thumbnailLink">Thumbnail Link</app-control-input>
                <app-control-input controlType="textarea" v-model="editedPost.content">Content</app-control-input>
                <app-button type="submit">Save</app-button>
                <app-button type="buttom" @click="onCancel">Cancel</app-button>
            </form>
        </section>
    </div>
</template>

<script>
import AppControlInput from '~/components/UI/AppControlInput.vue'
import AppButton from '~/components/UI/AppButton.vue'
export default {
    data() {
        return {
            editedPost: {
                author: '',
                title: '',
                thumbnailLink: '',
                content: ''
            }
        }
    },
    components: {
        AppControlInput,
        AppButton
    },
    methods: {
        onSave() {
            console.log(this.editedPost);
        },
        onCancel() {
            // navigate back
            // to access router, we need "this" as it's required to access injected properties
            this.$router.push('/admin');
        }
    }
    
}
</script>