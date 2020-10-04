<template>
  <router-link to="/portfolio">
    <button class="button"><slot></slot></button>
  </router-link>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Indie+Flower&display=swap');

.button {
  margin: 0, auto;
  padding: 20px;
  border: 2px solid #f7f7f7;
  text-align: center;
  text-transform: uppercase;
  font-size: 4rem;
  background: transparent;
  color: white;
  border-radius: 5% 5% 5% 25%;
  font-family: 'Indie Flower', cursive;

  position: absolute;
  @include absoluteCenter;
  top: 65%;

  overflow: hidden;
  transition: .3s;

  &:after {
    position: absolute;
    transition: .3s;
    content: '';
    width: 0;
    height: 120%;
    left: -10%;
    bottom: 0;
    height: 3px;
    background: #f7f7f7;

    transform: skewX(15deg);
    z-index: -1;
  }

  &:hover {
    cursor: pointer;
    color: #5bcaff;
    &:after {
        width: 120%;
        left: -10%;
    }
  }
}


</style>>

