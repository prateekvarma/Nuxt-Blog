<template>
    <div>
        <nuxt-link :to="'/posts/' + id">
          <article>
            <div>
              <h1>{{ title }}</h1>
              <p>{{ previewText }}</p>
              <div :style="{backgroundImage: 'url(' + thumbnail + ')' }"></div>
            </div>
          </article>
        </nuxt-link>
    </div>
</template>

<script>
export default {
    name: 'PostPreview',
    props: {
        id: {
            type: String,
            required: true
        },
        title: {
            type: String,
            required: true
        },
        previewText: {
            type: String,
            required: true
        },
        thumbnail: {
            type: String,
            required: true
        }
    }
}
</script>