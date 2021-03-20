<template>
  <div>
    <div v-for="e in errata" :key="e.slug">
      <nuxt-link :to="'errata/'+ e.slug">{{e.title}}</nuxt-link>
    </div>
  </div>
</template>

<script>

export default {
  async asyncData ({ $content, params }) {
    const query = await $content('errata' || 'index').limit(15)
    const errata = await query.fetch()
    return { errata }
  }
}
</script>
