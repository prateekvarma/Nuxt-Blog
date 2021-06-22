<template>
  <div class="container">
    <div>
      <h1 class="title">
        Nuxt Blog
      </h1>
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
    </div>
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

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

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

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
