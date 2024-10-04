<script>
import { faker } from '@faker-js/faker';

export default {
  name: "ProfileCard",
  data() {
    return {
      fullName: faker.name.fullName(),
      email: faker.internet.email(),
      city: faker.address.city(),
      country: faker.address.country()
    };
  }
};
</script>


<template>
  <div class="p-4 bg-white rounded-lg shadow-md">
    <h2 class="text-xl font-bold">{{ fullName }}</h2>
    <p>Email: {{ email }}</p>
    <p>Location: {{ city }}, {{ country }}</p>
  </div>
</template>



