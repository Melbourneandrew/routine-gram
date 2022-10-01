<template>
  <div class="tl">
    <div class="head-row">
      <h1 class="title">Todays Schedule</h1>
      <img class="logo" src="/logo.png" />
    </div>
    <v-timeline class="timeline" side="end" truncate-line="end">
      <v-timeline-item
        dot-color="primary"
        size="x-large"
        icon="mdi-octagram-outline"
        icon-color="white"
      >
        <div class="d-flex">
          <strong class="mr-4">8am</strong>
          <div>
            <strong>Meditate</strong>
            <div class="text-caption">Heartful</div>
          </div>
        </div>
      </v-timeline-item>

      <v-timeline-item
        dot-color="teal-lighten-3"
        size="x-large"
        icon="mdi-calendar"
        icon-color="white"
      >
        <div class="d-flex">
          <strong class="mr-4">9-11am</strong>
          <div>
            <strong>Design Stand Up</strong>
            <div class="text-caption mb-2">MS Teams</div>
          </div>
        </div>
      </v-timeline-item>

      <v-timeline-item dot-color="pink" size="large">
        <div class="d-flex">
          <strong class="mr-4">12pm</strong>
          <div>
            <strong>Lunch break</strong>
          </div>
        </div>
      </v-timeline-item>

      <v-timeline-item
        dot-color="teal-lighten-3"
        size="x-large"
        icon="mdi-calendar"
        icon-color="white"
      >
        <div class="d-flex">
          <strong class="mr-4">2-3pm</strong>
          <div>
            <strong>Go Climbing</strong>
            <div class="text-caption">Summit</div>
          </div>
        </div>
      </v-timeline-item>

      <v-timeline-item
        dot-color="teal-lighten-3"
        size="x-large"
        icon="mdi-calendar"
        icon-color="white"
      >
        <div class="d-flex">
          <strong class="mr-4">5pm</strong>
          <div>
            <strong>Consultant Onboarding</strong>
            <div class="text-caption">MS Teams + Jira</div>
          </div>
        </div>
      </v-timeline-item>

      <v-timeline-item
        dot-color="primary"
        size="x-large"
        icon="mdi-octagram-outline"
        icon-color="white"
      >
        <div class="d-flex">
          <strong class="mr-4">6pm</strong>
          <div>
            <strong>Cook Nutritious Meal</strong>
            <div class="text-caption">Low carb!!</div>
          </div>
        </div>
      </v-timeline-item>

      <v-timeline-item
        dot-color="teal-lighten-3"
        size="x-large"
        icon="mdi-calendar"
        icon-color="white"
      >
        <div class="d-flex">
          <strong class="mr-4">7pm</strong>
          <div>
            <strong>Work on FPV drone</strong>
            <div class="text-caption">Tune PID</div>
          </div>
        </div>
      </v-timeline-item>

      <v-timeline-item
        dot-color="teal-lighten-3"
        size="x-large"
        icon="mdi-calendar"
        icon-color="white"
      >
        <div class="d-flex">
          <strong class="mr-4">11:30pm</strong>
          <div>
            <strong>Bedtime</strong>
            <div class="text-caption">Set alarm</div>
          </div>
        </div>
      </v-timeline-item>
    </v-timeline>
  </div>
</template>

<script setup>
</script>
<style scoped>
.timeline {
  margin-left: -30px;
  font-size: 20px;
}

.title {
  margin-top: 40px;
  margin-bottom: 20px;
}
.head-row {
  display: flex;
  align-items: center;
}
.logo {
  margin: auto;
  margin-right: 20px;
  margin-top: 30px;
  width: 60px;
  height: 60px;
}
</style>
