<template>
  <div class="navbar" >
    <div class="nav-item" @click="navigateBuildTodo">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        :width="size"
        :height="size"
        fill="currentColor"
        class="bi bi-pen"
        viewBox="0 0 16 16"
      >
        <path
          d="m13.498.795.149-.149a1.207 1.207 0 1 1 1.707 1.708l-.149.148a1.5 1.5 0 0 1-.059 2.059L4.854 14.854a.5.5 0 0 1-.233.131l-4 1a.5.5 0 0 1-.606-.606l1-4a.5.5 0 0 1 .131-.232l9.642-9.642a.5.5 0 0 0-.642.056L6.854 4.854a.5.5 0 1 1-.708-.708L9.44.854A1.5 1.5 0 0 1 11.5.796a1.5 1.5 0 0 1 1.998-.001zm-.644.766a.5.5 0 0 0-.707 0L1.95 11.756l-.764 3.057 3.057-.764L14.44 3.854a.5.5 0 0 0 0-.708l-1.585-1.585z"
        />
      </svg>
    </div>
    <div class="nav-item" @click="navigateSchedule">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        :width="size"
        :height="size"
        fill="currentColor"
        class="bi bi-calendar4-week"
        viewBox="0 0 16 16"
      >
        <path
          d="M3.5 0a.5.5 0 0 1 .5.5V1h8V.5a.5.5 0 0 1 1 0V1h1a2 2 0 0 1 2 2v11a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V3a2 2 0 0 1 2-2h1V.5a.5.5 0 0 1 .5-.5zM2 2a1 1 0 0 0-1 1v1h14V3a1 1 0 0 0-1-1H2zm13 3H1v9a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1V5z"
        />
        <path
          d="M11 7.5a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-1a.5.5 0 0 1-.5-.5v-1zm-3 0a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-1a.5.5 0 0 1-.5-.5v-1zm-2 3a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-1a.5.5 0 0 1-.5-.5v-1zm-3 0a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-1a.5.5 0 0 1-.5-.5v-1z"
        />
      </svg>
    </div>
    <div class="nav-item" @click="navigateFeed">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        :width="size"
        :height="size"
        fill="currentColor"
        class="bi bi-collection"
        viewBox="0 0 16 16"
      >
        <path
          d="M2.5 3.5a.5.5 0 0 1 0-1h11a.5.5 0 0 1 0 1h-11zm2-2a.5.5 0 0 1 0-1h7a.5.5 0 0 1 0 1h-7zM0 13a1.5 1.5 0 0 0 1.5 1.5h13A1.5 1.5 0 0 0 16 13V6a1.5 1.5 0 0 0-1.5-1.5h-13A1.5 1.5 0 0 0 0 6v7zm1.5.5A.5.5 0 0 1 1 13V6a.5.5 0 0 1 .5-.5h13a.5.5 0 0 1 .5.5v7a.5.5 0 0 1-.5.5h-13z"
        />
      </svg>
    </div>
  </div>
</template>

<script setup>
import router from '@/router';

    const size = 38;
    function navigateBuildTodo(){
        router.push({path:'/'})
    }
    function navigateSchedule(){
        router.push({path:'/schedule'})
    }
    function navigateFeed(){
        router.push({path:'/feed'})
    }
</script>
<style scoped>
.navbar {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  display: flex;
  flex-direction: row;
  padding: 5px;
  padding-bottom: 10px;
  padding-top: 10px;
  background-color: white;
  z-index: 1000;

}
.nav-item {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: auto;
  background-color: white;
  z-index: 1000;
}
</style>
