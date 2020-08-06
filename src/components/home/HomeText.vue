<template>
  <div class="homecont">
    <div class="hometxt">
      <p class="p1">Buy your new car</p>
      <p class="p2">Or just pretend you buy</p>
    </div>
    <div class="homebuttons">
      <router-link tag="button" to="/" class="b1">Sign UP</router-link>
      <router-link tag="button" to="/" class="b2">Sign IN</router-link>
    </div>
  </div>
</template>

<style>
.homecont {
  width: 60vw;
  height: 45vh;
  text-align: center;
}

.p1::selection {
  background: black;
}

.p2::selection {
  background: black;
}

.b1 {
  background-color: #eee;
  width: 10vw;
  height: 5.5vh;
  border: 1px solid #eee;
  border-radius: 10px;
  font-size: 22px;
  font-weight: bold;
  text-transform: uppercase;
  margin-right: 4vw;
  color: #ff0000;
  outline: none;
  -webkit-box-shadow: -9px -9px 9px 0px rgba(255, 134, 134, 0.4),
    9px 9px 9px 0px rgba(65, 65, 65, 0.35);
  -moz-box-shadow: -9px -9px 9px 0px rgba(255, 134, 134, 0.4),
    9px 9px 9px 0px rgba(65, 65, 65, 0.35);
  box-shadow: -9px -9px 9px 0px rgba(255, 134, 134, 0.4),
    9px 9px 9px 0px rgba(65, 65, 65, 0.35);
}

.b2 {
  background-color: #f91616;
  width: 10vw;
  height: 5.5vh;
  border: 1px solid #f91616;
  border-radius: 10px;
  font-size: 22px;
  font-weight: bold;
  text-transform: uppercase;
  color: #ededed;
  -webkit-box-shadow: -9px -9px 9px 0px rgba(255, 134, 134, 0.4),
    9px 9px 9px 0px rgba(65, 65, 65, 0.35);
  -moz-box-shadow: -9px -9px 9px 0px rgba(255, 134, 134, 0.4),
    9px 9px 9px 0px rgba(65, 65, 65, 0.35);
  box-shadow: -9px -9px 9px 0px rgba(255, 134, 134, 0.4),
    9px 9px 9px 0px rgba(65, 65, 65, 0.35);
}

.b1:focus {
  -webkit-box-shadow: inset 5px 5px 5px 0px rgba(65, 65, 65, 0.25),
    inset -5px -5px 5px 0px rgba(255, 255, 255, 1);
  -moz-box-shadow: inset 5px 5px 5px 0px rgba(65, 65, 65, 0.25),
    inset -5px -5px 5px 0px rgba(255, 255, 255, 1);
  box-shadow: inset 5px 5px 5px 0px rgba(65, 65, 65, 0.25),
    inset -5px -5px 5px 0px rgba(255, 255, 255, 1);
}

.b2:focus {
  -webkit-box-shadow: inset 10px 10px 15px 0px rgba(65, 65, 65, 0.12),
    inset -10px -10px 15px 0px rgba(255, 134, 134, 0.4);
  -moz-box-shadow: inset 10px 10px 15px 0px rgba(65, 65, 65, 0.12),
    inset -10px -10px 15px 0px rgba(255, 134, 134, 0.4);
  box-shadow: inset 10px 10px 15px 0px rgba(65, 65, 65, 0.12),
    inset -10px -10px 15px 0px rgba(255, 134, 134, 0.4);
  transform: scale(0.98);
}

button:focus {
  outline: 0;
}

.p1 {
  font-size: 80px;
  color: #ededed;
  font-weight: bold;
}

.p2 {
  font-size: 30px;
  color: #bebdbd;
  font-weight: bold;
  padding: 0 0 2.5vh 0;
  margin-top: -2vh;
}
</style>
