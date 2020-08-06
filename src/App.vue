<template>
  <b-container fluid style="padding: 0">
    <app-header style="position: absolute"></app-header>
    <router-view></router-view>
  </b-container>
</template>

<script>
import header from "@/components/Header.vue";

export default {
  components: {
    appHeader: header
  }
};
</script>

<style>
body {
  background-color: #eee;
  margin: 0;
  text-transform: uppercase;
}
</style>
