<template>
    <div class="card card-display">
        <img src="../../assets/newyord.png" class="card-img-top circle-card" alt="...">
        <div class="card-body">
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
                content.
            </p>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../../assets/main' as *;
.card-display{
          @include FlexDisplay(column, normal, center, 100%, auto);
          border: none;
        }
        .circle-card{
          border-radius: 50%;
          width: 30%;
          height: 30%
        }
    
</style>