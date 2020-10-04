<template>
  <div class="col-1-of-2 project">
      <div class="project__item">
          <img :src="/img/ + project.img" alt="StupidPieceOfShit" class="project__img">
          <div class="project__overlay">
              <div class="project__buttons">
                  <button href="#" class="project__button">
                      <font-awesome-icon icon="eye" />
                  </button>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>