<script lang="ts" setup>


import Recipecard from '~/components/Recipecard.vue';
import { type RecipeResponse } from"../types/types"
const {data , error}= await useFetch<RecipeResponse>("https://dummyjson.com/recipes")
</script>

<template>
  <div>
    
    <section class="py-20 container">
      <h2 class="text-3xl lg:text-5xl mb-2">TESTY AND DELYICIOUS </h2>
      <p class="text-lg lg:text-xl mb-8">Check out our most popular recipes! </p>
      <!-- condition makeing -->
      <div v-if="!error" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-x-4 gap-y-8">
       <Recipecard v-for="recipe in data?.recipes " :recipe="recipe"></Recipecard>
      </div> 
      <p v-else class="text-xl"> Opss ,Something went wrong .Please tru again leter</p>
    </section>
    

  </div>
   
</template>


