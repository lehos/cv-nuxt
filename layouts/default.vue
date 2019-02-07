<script>
export default {}
</script>

<template>
  <div class="layout">
    <header>
      <h1>{{$t('title')}}</h1>
      <nav>
        <nuxt-link to="/">ru</nuxt-link>
        |
        <nuxt-link to="/en/">en</nuxt-link>
      </nav>
    </header>
    <nuxt/>
  </div>
</template>
