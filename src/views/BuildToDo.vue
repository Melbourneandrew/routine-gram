<template>
  <div class="buildTodo">
    <img class="logo" src="/logo.png" />
    <h1 class="title">What do you want to do today?</h1>
    <textarea
      class="tasksInput"
      placeholder="Enter some tasks..."
    ></textarea>
    <div class="nav-button" @click="navigate">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="48"
        height="48"
        fill="currentColor"
        class="bi bi-arrow-right"
        viewBox="0 0 16 16"
      >
        <path
          fill-rule="evenodd"
          d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"
        />
      </svg>
    </div>
  </div>
</template>

<script setup>
import router from "@/router";

function navigate() {
  router.push({ path: "/schedule" });
}
</script>
<style scoped>
.buildTodo {
  width: 100%;
  height: fit-content;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: left;
  padding-top: 100px;
}

.title {
  width: 100%;
  text-align: left;
  padding-left: 30px;
}

.tasksInput {
  width: 90%;
  height: 250px;
  border-radius: 15px;
  border-color: gray;
  border-width: 1px;
  border-style: solid;
  padding: 14px;
  font-size: 20px;
  margin-top: 30px;
}

.nav-button {
  border-style: solid;
  border-color: black;
  border-width: 2px;
  border-radius: 10px;
  padding: 8px;
  display: flex;
  justify-content: center;
  align-items: center;

  margin-top: 60px;
}
</style>
