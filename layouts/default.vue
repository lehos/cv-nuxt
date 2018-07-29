<template>
  <div>
    <header class="Header">
      <div class="container">
        <h1 class="Header__Title">{{$t('title')}}</h1>
        <nav class="Header__Menu">
          <nuxt-link :to="`/en` + $route.fullPath" exact>
            en
          </nuxt-link>
          |
          <nuxt-link :to="$route.fullPath.replace(/^\/[^\/]+/, '')"  exact>
            ru
          </nuxt-link>
        </nav>
      </div>
    </header>
    <nuxt/>
  </div>
</template>

<script>
  export default {}
</script>

