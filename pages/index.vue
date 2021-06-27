<template>
  <div class="container">
    <div>
      <h1 class="title">
        Nuxt Blog
      </h1>
      <post-list />
    </div>
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

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
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
