<template>
    <button :style="{ background: color }" @click="result()">{{ text }}</button>
</template>

<script>
    export default {
        name: "ButtonCom",
        props: {
            text: String,
            color: String
        },
        methods:{
            result(){
                console.log("hey")
            }
        }
    }
</script>