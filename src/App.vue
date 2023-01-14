<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header/Header.vue';

</script>

<template>
  
  <Header></Header>
  <RouterView />
  <footer>
    <h5>Copyright Company, inc 2021</h5>
  </footer>
</template>

<style lang="scss" scoped>
@use '../src/assets/main' as *;
  
  footer{
    @include FlexDisplay(row, flex-start, center, 100%, auto);
    border-top: 1px solid;
    h5{
      padding: 2%;

    }
  }
</style>
