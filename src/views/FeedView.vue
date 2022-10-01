<template>
  <div class="feed">
    <h1 class="title">Feed</h1>
    <Post v-for="(user, index) in users" :key="index" :user="user" />
  </div>
</template>

<script setup>
import Post from "../components/OnePost.vue";

const users = [
    {
        name: "John",
        description: "Father. Sales Associate. Adventurer",
        habits: [
            {
                title: "Meditate",
                cal: false
            },
            {
                title: "2 Mile Run",
                cal: false
            },
            {
                title: "Performance Review",
                cal: true
            }
        ]
    },
    {
        name: "Erin",
        description: "CS Student. Gamer",
        habits: [
            {
                title: "Stretch Wrists",
                cal: false
            },
            {
                title: "Water plants",
                cal: false
            },
            {
                title: "Physics Lab",
                cal: true
            }
        ]
    },
    {
        name: "Marc",
        description: "Father. Entrepreneur.",
        habits: [
            {
                title: "Resistance Training",
                cal: false
            },
            {
                title: "Affirmations",
                cal: false
            },
            {
                title: "Film Shark Tank",
                cal: true
            }
        ]
    },
    {
        name: "Andrew",
        description: "Software Engineer. Drone Pilot",
        habits: [
            {
                title: "Exercise",
                cal: false
            },
            {
                title: "Hackathon",
                cal: true
            },
            {
                title: "Dinner @ Moxies",
                cal: true
            }
        ]
    }
]
/**
 * Walks
 * gratitude journaling
 * yoga
 * cook dinner
 * drink 1 gal water
 * water plants
 * call loved one
 * 
 */
</script>
<style scoped>
.feed {
  width: 100%;
  height: fit-content;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 200px;
}
.title {
  margin-top: 40px;
  margin-bottom: 20px;
}
</style>
