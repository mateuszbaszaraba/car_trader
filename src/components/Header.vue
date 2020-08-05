<template>
  <div>
    <b-button v-b-toggle.sidebar-1>Toggle Sidebar</b-button>
    <b-sidebar id="sidebar-1" shadow>
      <slot name="title"></slot>
      <template v-slot:title>
        <h3 class="mt-1"><span style="color: red">Car</span>Trader</h3>
      </template>
      <div class="px-3 py-2 menu-cont">
        <router-link tag="p" to="/" class="menu-item">Home</router-link>
        <router-link tag="p" to="/portfolio" class="menu-item"
          >Portfolio</router-link
        >
        <router-link tag="p" to="/cars" class="menu-item">Cars</router-link>
      </div>
    </b-sidebar>
  </div>
</template>

<style>
.menu-item {
  cursor: pointer;
  height: 12vh;
  font-size: 5vh;
  text-align: center;
}

.menu-cont {
  margin-top: 8vh;
  height: 70vh;
  display: flex;
  justify-content: space-around;
  flex-direction: column;
  transition: 0.5s;
}

.menu-item:hover {
  text-decoration: line-through;
}
</style>
