<template>
  <router-link to="/portfolio" class="button">
    <button class="button_top"><slot></slot></button>
    <button class="button_bottom"><slot></slot></button>
  </router-link>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.button {
  display: block;
  margin: auto;
  margin-top: 8rem;
  height: 5rem;
  width: 16rem;
  overflow: hidden;
  text-decoration: none;
  
  *
  {
    transition: all 150ms;
    display: block;
    width: 100%;
    height: 4.5rem;
    line-height: 1;
    font-size: 2rem;
    border: 2px solid white;
    background-color: red;
    color: white;
    font-family: Staatliches, sans-serif;
  }
  
  &_bottom {
    margin-top: 1rem;
    background-color: white;
    color: green;
  }
  
  &:hover * {
    transform: translateY(-5.5rem);
    cursor: pointer;
  }
  
}


</style>>

