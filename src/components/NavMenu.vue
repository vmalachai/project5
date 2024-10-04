<template>
  <nav class="bg-blue-500 p-4 text-white">
    <ul class="flex justify-center space-x-4">
      <li>
        <router-link to="/" class="hover:underline" active-class="underline underline-offset-4">
          Home
        </router-link>
      </li>
      <li>
        <router-link to="/other" class="hover:underline" active-class="underline underline-offset-4">
          Other
        </router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "NavMenu",
};
</script>
