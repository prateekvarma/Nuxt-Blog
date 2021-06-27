<template>
    <div class="links">
    <post-preview 
        id="1"
        thumbnail="https://t3.ftcdn.net/jpg/03/46/83/96/360_F_346839683_6nAPzbhpSkIpb8pmAwufkC7c5eD7wYws.jpg"
        title="First title"
        previewText="First Preview Text"
    />
    <post-preview 
        id="2"
        thumbnail="https://t3.ftcdn.net/jpg/03/46/83/96/360_F_346839683_6nAPzbhpSkIpb8pmAwufkC7c5eD7wYws.jpg"
        title="Second title"
        previewText="Second Preview Text"
    />
    </div>
</template>

<script>
import PostPreview from '~/components/Posts/PostPreview.vue'
export default {
    components: {
        PostPreview
    }
}
</script>

<style scoped>
.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>