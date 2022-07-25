<template>
  <h1>Superfast Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <router-link :to="{ name: 'JobDetails', params: { id: job.id }}">
      <h3>{{ job.title }}</h3>
    </router-link>  
  </div>
</template>

<script>
export default {
    data() {
        return {
            jobs: [
                {title: 'Superfast UX Designer', id: 1, details: 'lorem'},
                {title: 'Superfast Web Developer', id: 2, details: 'lorem'},
                {title: 'Superfast Vue Designer', id: 3, details: 'lorem'},
            ]
        }
    }
}
</script>

<style>

</style>