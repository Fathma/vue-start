<template>
    <h3>TESDGFJHSFDJ</h3>
    <div :key="task.id" v-for="task in tasks">
        <h3>{{ task.text }}</h3>
    </div>
</template>

<script>
    export default {
        name: "TasksCom",
        props: {
            tasks: Array
        }
    }
</script>