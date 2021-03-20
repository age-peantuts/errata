<template>
  <article>
    <h1>{{errata.title}}</h1>
    <dl>
      <dt>date</dt>
      <dd>{{errata.date}}</dd>
    </dl>

    <nuxt-content :document="errata" />
  </article>
</template>

<script>
export default {
  async asyncData ({ $content, params }) {
    const errata = await $content('errata', params.slug || 'index').fetch()
    return { errata }
  }
}
</script>
