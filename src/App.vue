<template>
  <b-container fluid>
    <app-header></app-header>
  </b-container>
</template>

<script>
import header from "@/components/Header.vue";

export default {
  components: {
    appHeader: header,
  },
};
</script>

<style>
body {
  background-color: red;
}
</style>
