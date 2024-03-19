<template>
  <Header />
  <div class="taskClass">
    <DailyTasks />
    <WeeklyTasks />
    <MonthlyTasks />
  </div>

</template>

<script setup>

import Header from './components/Header.vue'
import DailyTasks from './components/DailyTasks.vue'
import WeeklyTasks from './components/WeeklyTasks.vue'
import MonthlyTasks from './components/MonthlyTasks.vue'
</script>

<style>
body {
  padding: 0% 5% 0% 5%;
  height: 100vh;
}

.taskClass {
  display: flex;
  width: 100%;
  height: 80vh;
}

.tasks {
  width: 100%;
  height: 100%;
  text-align: center;
  border-left: solid 3px #ccc;
  border-right: solid 3px #ccc;
}

input {
  width: 90%;
  height: 50px;
  padding: 10px;
  border-radius: 6px;
  border: solid 3px #ccc;
}

input:focus {
  border: solid 4px pink;
}

ul {
  list-style-type: none;
  width: 100%;
  padding: 2%;
}

li {
  width: 90%;
  text-align: left;
  color: white;
  margin: 5px 0px 5px 0px;
  background-color: grey;
  padding: 10px;
}
</style>
