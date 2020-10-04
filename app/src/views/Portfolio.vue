<template>
  <main>
    <secondary-header-component></secondary-header-component>
    <secondary-sub-component></secondary-sub-component>
    <projects-component></projects-component>
  </main>
</template>

<script>
// @ is an alias to /src

import SecondaryHeaderComponent from '@/components/SecondaryHeaderComponent'
import SecondarySubComponent from '@/components/SecondarySubComponent'
import ProjectsComponent from '@/components/ProjectsComponent'
export default {
  components: {SecondaryHeaderComponent, SecondarySubComponent, ProjectsComponent},
  data() {
    return {
      loading: true
    }
  },

  mounted() {
    setTimeout(() => {
      this.loading = false;
    }, 200)
  }
}
</script>


<style lang="scss" scoped>

</style>