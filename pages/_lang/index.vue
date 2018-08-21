<script>
export default {
  data() {
    return {
      skills: this.$t('skills'),
      jobs: this.$t('jobs')
    }
  },
}
</script>

<template>
  <div>
    <h2>{{$t('about.header')}}</h2>
    <p>{{$t('about.text')}}</p>

    <h2>{{$t('skills-header')}}</h2>
    <div v-for="(skill, index) in skills" :key="`skill${index}`">
      {{skill}}
    </div>

    <h2>{{$t('jobs-header')}}</h2>
    <div v-for="(job, index) in jobs" :key="`job${index}`">
      <div class="job-date">{{job.date}}</div>
      <div class="job-company" v-html="job.company"></div>
      <div class="job-position">{{job.position}}</div>
      <ul>
        <li v-for="(desc, index) in job.desc" :key="`desc${index}`" v-html="desc"></li>
      </ul>
      <div class="job-stack">
        {{job.stack}}
      </div>
    </div>
  </div>
</template>
