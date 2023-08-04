<template>
  <div class="app">
    <p>{{ name }} - {{ age }}</p>
    <button @click="changeName('Afia')">Change Name</button>
    <button @click="changeAge('25')">Change Age</button>
    <button @click="changeAge(24)">Change Age</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {},
  data() {
    return {
      name: "Asif",
      age: 28 as number | string
    }
  },
  methods: {
    changeName(name: string) {
      this.name = name
    },
    changeAge(age: number | string) {
      this.age = age
    }
  }
});
</script>

<style>

</style>