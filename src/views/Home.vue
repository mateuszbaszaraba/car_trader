// @ is an alias to /src
<template>
  <div class="ccontainer">
    <app-home-text></app-home-text>
  </div>
</template>

<script>
import homeText from "@/components/home/HomeText.vue";

export default {
  components: {
    appHomeText: homeText
  }
};
</script>

<style>
.ccontainer {
  width: 100vw;
  height: 100vh;
  background-color: red;
  clip-path: polygon(100% 0, 100% 88%, 43% 100%, 0 100%, 0 0);
  z-index: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
