<template>
  <div style="z-index: 1">
    <div class="hamburger" v-b-toggle.sidebar-1>
      <div class="hamb"></div>
      <div class="hamb"></div>
      <div class="hamb"></div>
    </div>
    <b-sidebar id="sidebar-1" shadow backdrop-variant="dark" backdrop>
      <slot name="title"></slot>
      <template v-slot:title>
        <router-link tag="h3" class="mt-2 ml-1" to="/" style="cursor: pointer">
          <span style="color: red">Car</span>Trader
        </router-link>
      </template>
      <div class="px-3 py-2 menu-cont">
        <router-link tag="p" to="/" class="menu-item">Home</router-link>
        <router-link tag="p" to="/portfolio" class="menu-item">Portfolio</router-link>
        <router-link tag="p" to="/cars" class="menu-item">Cars</router-link>
      </div>
    </b-sidebar>
  </div>
</template>

<style>
button {
  outline: none;
}

#sidebar-1 {
  border-radius: 0px 15px 15px 0px;
  -moz-border-radius: 0px 15px 15px 0px;
  -webkit-border-radius: 0px 15px 15px 0px;
  border: 0px solid #000000;
}

.menu-item {
  cursor: pointer;
  height: 12vh;
  font-size: 5vh;
  text-align: center;
  color: rgb(94, 94, 94);
}

.menu-cont {
  margin-top: 9vh;
  height: 70vh;
  display: flex;
  justify-content: space-around;
  flex-direction: column;
  transition: 0.5s;
}

.menu-item:hover {
  text-decoration: line-through;
}

.hamb {
  width: 3.1vw;
  height: 5px;
  background-color: white;
  margin: 6px 0;
  outline: none;
}

.hamburger {
  margin: 5vh 0 0 3vw;
  width: 3.1vw;
  outline: none;
}
</style>
