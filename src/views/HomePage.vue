<script setup>
import { ref } from 'vue';
import RecipeCard from '@/components/RecipeCard.vue';
import ProfileCard from '@/components/ProfileCard.vue';

const title = ref('Welcome to the Home Page');
</script>

<template>
  <main class="min-h-screen p-8 bg-gray-100">
    <!-- Title section -->
    <section class="flex items-center justify-center mb-8">
      <h1 class="text-6xl font-thin text-slate-800">{{ title }}</h1>
    </section>

    <!-- Recipe and Profile Cards section -->
    <section class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
      <!-- Example of displaying multiple Recipe and Profile cards -->
      <RecipeCard v-for="i in 3" :key="'recipe-' + i" />
      <ProfileCard v-for="i in 3" :key="'profile-' + i" />
    </section>
  </main>
</template>


