<template>
  <div>
    <introduction-component></introduction-component>
    <button-component>View Projects</button-component>
  </div>
</template>

<script>
import IntroductionComponent from '@/components/IntroductionComponent'
import ButtonComponent from '@/components/ButtonComponent'


export default {
  components: {
    IntroductionComponent,
    ButtonComponent
  }
}
</script>