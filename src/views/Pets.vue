<template>
  <v-container grid-list-md fluid>
    <v-layout wrap>
      <v-flex xs12 sm4 md3 v-for="pet in dogs" :key="pet.breed"> </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import { Dogs } from "../data/dogs";
import Dog from "../components/Dog.vue";
export default {
  components: {
    appDog: Dog
  },
  data() {
    return {
      dogs: Dogs
    };
  }
};
</script>

<style scoped>
p {
  margin: 0;
}
</style>
