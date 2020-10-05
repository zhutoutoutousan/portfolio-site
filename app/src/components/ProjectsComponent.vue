<template>
  <div class="portfolio">
      <div class="row">
        <project-component :project="projects.chessGame" :class="{'slide-left':loading}"></project-component>
        <project-component :project="projects.portfolio" :class="{'slide-right':loading}"></project-component>
      </div>
      <div class="row">
        <project-component :project="projects.studyFramework" :class="{'slide-left':loading}"></project-component>
      </div>
  </div>
</template>

<script>
import ProjectComponent from '@/components/ProjectComponent'

export default {
  components: { ProjectComponent },
  data() {
    return {
      loading: true,
      projects: {
        chessGame: {
          name: 'Chess game',
          summary: 'Lorem ipsum',
          img: 'chess-game.png',
          demo: 'https://mxxtherfxxing-chess-game.herokuapp.com/',
          code: 'https://github.com/zhutoutoutousan/chess-game',
          technologies: [
            {name: 'ES6'},
            {name: 'Object Oriented Programming'},
            {name: 'p5.js'},
            {name: 'Express'},
            {name: 'Node.js'}
          ]
        },
        portfolio: {
          name: 'Portfolio',
          summary: 'Lorem ipsum',
          img: 'studynote.png',
          demo: '',
          code: '',
          technologies: [
            {name: 'HTML & CSS'},
            {name: 'JavaScript'},
            {name: 'SASS'},
            {name: 'Vue.JS'},
            {name: 'Responsive'},
            {name: 'UI/UX'},
          ]
        },
        studyFramework: {
          name: 'Study Note',
          summary: 'Lorem ipsum',
          img: 'studynode.png',
          demo: 'https://warm-oasis-28882.herokuapp.com/',
          code: 'https://github.com/zhutoutoutousan/A-study-note-as-a-beginner',
          technologies: [
            {name: 'Markdown'},
          ]
        }
      }
    }
  },
  mounted() {
    setTimeout(() => {
      this.loading =false
    }, 400)
  }
}
</script>

<style>
  .portfolio {margin-top: 4rem;}

  .slide-left {
    opacity: 0;
    visibility: hidden;
    transform: translateX(-5rem);
  }

  .slide-right {
    opacity: 0;
    visibility: hidden;
    transform: translateX(5rem);
  }
</style>