<template>
  <div class="introduction">world.create("Tian Shao").run()
      <br>
      $Shanghai; 
      <br>
      $web-development;
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap');
.introduction
{
    @include absoluteCenter;

    font-family: 'Permanent Marker', cursive;
    text-align: center;
    color: rgb(105, 66, 66);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    letter-spacing: 5px;

    background-image: url(https://media.giphy.com/media/553Zs1KrXN7A3H7ofT/giphy.gif);
    background-size: cover;
    color: transparent;
    background-clip: text;
    -moz-background-clip: text;
    -webkit-background-clip: text;
    font-size: 8rem;

    @media only screen and (max-width: 62.5rem), (max-height: 47rem ) {
        font-size: 4rem;
    }

    @media only screen and (max-width: 78rem) {
        font-size: 4rem;
    }

    @media only screen and (max-width: 41rem) {
        font-size: 4rem;
    }
}
</style>>
