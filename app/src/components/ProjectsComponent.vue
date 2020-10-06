<template>
  <div class="portfolio">
      <div class="row">
        <project-component :project="projects.chessGame" :class="{'slide-left':loading}"></project-component>
        <project-component :project="projects.portfolio" :class="{'slide-right':loading}"></project-component>
      </div>
      <div class="row">
        <project-component :project="projects.studyFramework" :class="{'slide-left':loading}"></project-component>
        <project-component :project="projects.lotteryGame" :class="{'slide-left':loading}"></project-component>
      </div>
      <div class="row">
                <project-component :project="projects.rpmEstimation" :class="{'slide-left':loading}"></project-component>
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
          summary: 'I\'ve always been a fan of chess, I enjoy watching Magnus Carlsen and Hikaru Nakamura. And one day I decided to design my own chess game. I studied the minimax algorithm, used ES6 and a little bit of p5.js to help myself design the board.',
          img: 'chess-game.png',
          demo: 'https://mxxtherfxxing-chess-game.herokuapp.com/',
          code: 'https://github.com/zhutoutoutousan/chess-game',
          technologies: [
            {name: 'ES6'},
            {name: 'OOP'},
            {name: 'p5.js'},
            {name: 'Express'},
            {name: 'Node.js'}
          ]
        },
        portfolio: {
          name: 'Portfolio',
          summary: 'Having studied front-end full-time for a little more than 6 months, I built a website to showcase my work. I studied vue.js via "frontendmaster" and I\'m still studying react. This project gives me more grasp on responsive web design and vue project architecture.',
          img: 'portfolio.png',
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
          summary: 'I used to be a good bel canto singer, aspired to be an artist. I studied English, German, French, Italian, Russian back in junior high, and was having a dream of becoming a philosopher and a musician before meeting some existential crisis that prompted me to steer to engineering, transforming from an idealist to a realist. And for the last few years, I know there\'s no way I\'m going to survive without some kind of systematic study methods to manage my spur to manage my intellectual rigor or attempts. So I created this tool.',
          img: 'study.png',
          demo: 'https://warm-oasis-28882.herokuapp.com/',
          code: 'https://github.com/zhutoutoutousan/A-study-note-as-a-beginner',
          technologies: [
            {name: 'Node.js'},
            {name: 'Express'},
            {name: 'EJS'}
          ]
        },
        lotteryGame: {
          name: 'Lottery game',
          summary: 'This is probably the first web application I developed, during the free time I had when working as a test engineer in my first job. I just started learning HTML, JavaScript and CSS, I used a little bit of Vue, with no sense of project architecture in mind. My application survived the test at last. That was the beginning of my journey of web development.',
          img: 'lottery.png',
          demo: 'https://github.com/zhutoutoutousan/lottery-game',
          code:'https://github.com/zhutoutoutousan/lottery-game',
          technologies: [
            {name: 'vue.js'},
            {name: 'JavaScript'},
            {name: 'HTML'},
            {name: 'CSS'}
          ]
        },
        rpmEstimation: {
          name: 'NVH project',
          summary: 'I participated in a project that, for me, sounds impossible to complete: Build a motor control and data acquisition unit that takes in the vibration and rotating speed signal, perform STFFT(Short-time Fast Fourier Transform) then send them to the server for deep learning purposes. The difficulty was insane, stuck on a path-finding problem(later discovered) and I barely survived and graduated by ditching the technical difficulty and go for an MVR(Minimal Viable Result). I managed to recover some of my codes(I was mentally unstable)',
          img: 'nvh.png',
          demo: 'https://ieeexplore.ieee.org/abstract/document/9044105',
          code:'https://github.com/zhutoutoutousan/Indirect-sensor-estimation',
          technologies: [
            {name: 'C'},
            {name: 'Embedded system'},
            {name: 'Code Composer Studio'},
            {name: 'Matlab'},
            {name: 'LaTeX'},
            {name: 'python'}
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