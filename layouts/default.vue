<script>
export default {}
</script>

<template>
  <div>
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
