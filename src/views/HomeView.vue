<script setup>
import Cardcity from '../components/CardCities/Cardcity.vue';
import SimpleCard from '../components/CardCities/SimpleCard.vue';
import CardRestaurant from '../components/CardCities/CardRestaurant.vue';

</script>

<template>
  <main>
    <section class="cities">
      <div class="top-cities">
        <h1>Top cities</h1>
        <SimpleCard />
        <SimpleCard />
        <SimpleCard />
        <SimpleCard />
      </div>
      <section class="cities-cards-section">
        <div class="card-container">
          <Cardcity />
        </div>
        <div class="card-container">
          <Cardcity />
        </div>
        <div class="card-container">
          <Cardcity />
        </div>
        <div class="card-container">
          <Cardcity />
        </div>
        <div class="card-container">
          <Cardcity />
        </div>
        <div class="card-container">
          <Cardcity />
        </div>
      </section>
    </section>
    <section class="restaurants">
      <div class="card-container-restaurant">
        <CardRestaurant/>
      </div>
      <div class="card-container-restaurant">
        <CardRestaurant/>
      </div>
      <div class="card-container-restaurant">
        <CardRestaurant/>
      </div>
      <div class="card-container-restaurant">
        <CardRestaurant/>
      </div>
    </section>
  </main>
</template>
<style lang="scss" scoped>
@use '../src/assets/main' as *;
    main {
      @include FlexDisplay(column, normal, center, 100%, auto);
      
      .restaurants{
        @include FlexDisplay(row, space-evenly, center, 100%, auto);
        margin: 2%;

        .card-container-restaurant{
            width: 23%;
            height: auto;
        }
        
      }
  
      .cities {
        @include FlexDisplay(row, space-evenly, center, 95%, auto);
        margin-top: 10vh;
        .top-cities {
          @include FlexDisplay(column, normal, center, 20%, auto);
        }
  
        .cities-cards-section {
          @include FlexDisplay(row, space-evenly, center, 80%, auto);
          flex-wrap: wrap;
  
          .card-container {
            width: 30%;
            height: auto;
            margin: 2vh,0,2vh,0;
          }
        }
      }
    }
</style>
