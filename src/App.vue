<template>
  <router-view />
  <NavBar />
</template>
<script setup>
import NavBar from '@/components/NavBar.vue';
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Fredoka&display=swap");
* {
  font-family: "Fredoka", sans-serif;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
.title {
  width: 100%;
  text-align: left;
  padding-left: 30px;
}
.logo{
  width: 70px;
  height: 70px;
}
</style>
