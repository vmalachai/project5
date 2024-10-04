<script>
import { faker } from '@faker-js/faker';

export default {
  name: "RecipeCard",
  data() {
    return {
      dishName: faker.food.dish(),
      prepTime: faker.datatype.number({ min: 10, max: 60 }), // Random prep time
      calories: faker.datatype.number({ min: 200, max: 600 }) // Random calorie count
    };
  }
};
</script>

<template>
  <div class="p-4 bg-white rounded-lg shadow-md">
    <h2 class="text-xl font-bold">{{ dishName }}</h2>
    <p>Preparation Time: {{ prepTime }} minutes</p>
    <p>Calories: {{ calories }} kcal</p>
  </div>
</template>



