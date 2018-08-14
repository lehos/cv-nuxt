<script>
export default {
  created () {
    console.log(this.$t('skills'))
  }
}
</script>

<template>
  <div>
    <h2>{{$t('about.header')}}</h2>
    <p>{{$t('about.text')}}</p>

    <h2>{{$t('skills-header')}}</h2>
    <div v-for="(skill, index) in $t('skills')" :key="index">
      {{skill}}
    </div>
  </div>
</template>
