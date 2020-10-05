<template>
  <div class="introduction">world.create("Tian Shao").run()
      <br>
      $Shanghai; $web-development
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
    position: absolute;
    left: 17rem;
    top: -15rem;

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

    @media only screen and (max-width: 62.5rem) {
        transform: translateX(-6rem);
        font-size: 5rem;
    }

    @media only screen and (max-width: 78rem) {
        transform: translateX(-8rem);
        font-size: 5rem;
    }

    @media only screen and (max-width: 41rem) {
        transform: translateX(-14rem);
        font-size: 5rem;
    }
}
</style>>
