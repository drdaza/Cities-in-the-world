<script setup>
import { RouterLink, RouterView } from 'vue-router';
import Banner from './Banner.vue';
</script>
<template >
    <header>
    <div class="wrapper">
      <nav class="navbar navbar-expand-lg bg-light border">
        <div class="container-fluid separate-container">
          <a class="navbar-brand" href="#">Cities in the world</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item">
                <RouterLink class="nav-link" to="/">Home</RouterLink>
              </li>
              <li class="nav-item">
                <RouterLink class="nav-link" to="/about">About</RouterLink>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </div>
  </header>
  <div class="banner">
    <Banner></Banner>
  </div>
</template>
<style lang="scss" scoped>
@use '../src/assets/main' as *;
.separate-container{
    @include FlexDisplay(row, space-between, center, 100%, auto);
}

.border{
  border: 1px solid;
}


</style>