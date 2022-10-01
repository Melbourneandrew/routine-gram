<template>
  <v-card
    class="post mx-auto"
    max-width="344"
    variant="outlined"
  >
    <v-card-item>
      <div>
        <div class="text-h6 mb-1 post-title">
          {{ props.user.name }}'s Habits
        </div>
        <div class="text-caption post-text">
          {{props.user.description}}
        </div>
        <v-chip v-for="(habit, index) in props.user.habits" :key="index" 
        class="ma-2 habit" :color="[habit.cal ? 'teal' : 'primary']" variant="outlined" size="large">
          <v-icon v-if="habit.cal" start icon="mdi-calendar"></v-icon>
          <v-icon v-else start icon="mdi-octagram-outline"></v-icon>
          {{habit.title}}
        </v-chip>
        <!-- <v-chip class="ma-2 habit" color="primary" variant="outlined" size="large">
          <v-icon start icon="mdi-octagram-outline"></v-icon>
          2 Mile Run
        </v-chip>
        <v-chip class="ma-2 habit" color="teal" variant="outlined" size="large">
          <v-icon start icon="mdi-calendar"></v-icon>
          Performance Review
        </v-chip> -->
      </div>
    </v-card-item>
<!-- 
    <v-card-actions>
      <v-btn variant="outlined"> Button </v-btn>
    </v-card-actions> -->
  </v-card>
</template>

<script setup>
// eslint-disable-next-line no-undef
const props = defineProps({
  user: Object
});
console.log(props);
</script>
<style scoped>
.post {
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  border: none;
  width: 90%;
  margin-top: 25px;
}
.post-title {
  text-align: left;
  font-family: "Fredoka", sans-serif !important;
  font-weight: bold;
  font-size: 30px !important;
  margin: 15px;
}
.post-text {
  text-align: left;
  font-family: "Fredoka", sans-serif !important;
  font-size: 17px !important;
  margin-left: 15px;
  margin-bottom: 10px;
  margin-top: 10px;
}
.habit{
  width: 90%;
  font-size: 20px;

}
</style>
