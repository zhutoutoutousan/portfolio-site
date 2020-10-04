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

      <div class="project__background">
          <div class="project__model">
              <buton class="project__close">
                  <font-awesome-icon icon="times" />
              </buton>

              <div class="project__left">
                  <img src="" alt="" class="project__img--modal">
              </div>

              <div class="project__right">
                  <div class="project__label">Project</div>
                  <h3 class="project__name"></h3>
                  <ul class="project__technologies">
                      <li class="project__technology"></li>
                  </ul>
                  <div class="project__label">About</div>
                  <p class="project__summary">

                  </p>
                  <a href="" class="project__button project__button--modal">
                      <font-awesome-icon icon="eye" /> Demo
                  </a>
                  <button class="project__button project__button--modal">
                      <font-awesome-icon icon="code" />
                  </button>
                  <a href="" class="project__button project__button--modal">
                      <font-awesome-icon icon="code" /> code
                  </a>
              </div>
          </div>
      </div>
  </div>
</template>

<script>

export default {
    props: ['project'],
    data() {
        return {
            showProject: false
        }
    }
}
</script>

<style>

</style>