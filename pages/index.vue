<template>
  <div class="container">
    <div>
      <h1 class="title">
        Nuxt Blog
      </h1>
      <div class="links">
        <nuxt-link :to="'/posts/' + 1">
          <article>
            <div>
              <h1>Post 1 title</h1>
              <p>Post 1 text</p>
            </div>
          </article>
        </nuxt-link>
        <nuxt-link :to="'/posts/' + 2">
          <article>
            <div>
              <h1>Post 2 title</h1>
              <p>Post 2 text</p>
            </div>
          </article>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
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
