<script>
import NavMenu from './components/NavMenu.vue';
import RecipeCard from './components/RecipeCard.vue';
import ProfileCard from './components/ProfileCard.vue';

export default {
  name: "App",
  components: {
    NavMenu,
    RecipeCard,
    ProfileCard
  }
}; 
</script>

<template>
  
  <div class="min-h-screen bg-gray-100 p-8">
    <h1 class="text-3xl font-bold mb-8">Welcome to Project 5</h1>
    
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
      <RecipeCard v-for="i in 3" :key="i" />
      <ProfileCard v-for="i in 3" :key="'profile-' + i" />
    </div>
  </div>
</template>
