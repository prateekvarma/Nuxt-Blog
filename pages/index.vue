<template>
  <div class="container">
    <div>
      <h1 class="title">
        Nuxt Blog
      </h1>
      <post-list :posts="loadedPosts" />
    </div>
  </div>
</template>

<script>
import PostList from '~/components/Posts/PostList.vue'
export default {
  components: {
    PostList
  },
  data() {
    return {
      loadedPosts: [
        {
          id: '1',
          title: 'This is title one',
          previewText: 'This is thy first preview text yolo',
          thunbnail: 'https://t3.ftcdn.net/jpg/03/46/83/96/360_F_346839683_6nAPzbhpSkIpb8pmAwufkC7c5eD7wYws.jpg'
        },
        {
          id: '2',
          title: 'This is title two',
          previewText: 'This is thy second preview text',
          thunbnail: 'https://t3.ftcdn.net/jpg/03/46/83/96/360_F_346839683_6nAPzbhpSkIpb8pmAwufkC7c5eD7wYws.jpg'
        }
      ]
    }
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
