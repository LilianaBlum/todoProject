<template>
    <div class="tasks">
        <h2>Daily Tasks</h2>
        <input type="text" id="todoInput" placeholder="Add a new task..." @keyup.enter="addNewTask"
            v-model="newTaskInput">
        <ul>
            <li v-for="(task, index) in tasks" :key="index">{{ task }}</li>
        </ul>
    </div>
</template>

<script>

export default {
    data() {
        return {
            tasks: [],
            newTaskInput: "",
        }
    },
    methods: {
        addNewTask() {
            this.tasks.push(this.newTaskInput);
        }
    }
}

</script>