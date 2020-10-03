<template>
  <div class="introduction">world.create("Tian Shao").run()</div>
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
    left: 18rem;
    top: -3rem;

    font-family: 'Permanent Marker', cursive;
    text-align: center;
    color: rgb(105, 66, 66);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    letter-spacing: 5px;

    background-image: url(https://media.giphy.com/media/n3xSURtNE62t2/giphy.gif);
    background-size: cover;
    color: transparent;
    background-clip: text;
    -moz-background-clip: text;
    -webkit-background-clip: text;
    font-size: 8rem;

    @media only screen and (min-width: 200rem) {
        transform: translateX(1rem);
    }
}
</style>>
