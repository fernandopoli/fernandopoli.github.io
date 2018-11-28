<template>
  <section class="container">
    <div>
      <h1 class="title">
        {{title}}
      </h1>
      <h2 class="subtitle">
        Fernando Poli&#39;s Portfolio.
      </h2>
      <div class="links">
        <a
        href="https://nuxtjs.org/"
        target="_blank"
        class="button--green">Documentation</a>
        <a
        href="https://github.com/nuxt/nuxt.js"
        target="_blank"
        class="button--grey">GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  layout: 'intern',
  data () {
    return {
      title: 'Works'
    }
  },
  head () {
    return {
      title: this.title,
      meta: [
      { hid: 'Esta es el hid', name: 'Este es el name', content: 'Esta es la content description' }
      ]
    }
  }
}
</script>