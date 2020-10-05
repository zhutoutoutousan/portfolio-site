<template>
  <main>
    <secondary-header-component :class="{'slide-top': loading}"></secondary-header-component>
    <secondary-sub-component :class="{'slide-top': loading}"></secondary-sub-component>
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
    .slide-top
    {
        opacity: 0;
        visibility: hidden;
        transform: translateY(-5rem)
    }

</style>