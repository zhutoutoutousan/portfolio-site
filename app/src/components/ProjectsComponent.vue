<template>
  <div class="portfolio">
      <div class="row">
        <project-component></project-component>
      </div>
      <div class="row">

      </div>
  </div>
</template>

<script>
import ProjectComponent from '@/components/ProjectComponent'

export default {
  components: { ProjectComponent },
  data() {
    return {
      loading: true
    }
  }
}
</script>

<style>

</style>