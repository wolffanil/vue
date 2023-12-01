<script>
    export default {
        data() {
            return {
                text7: ''
            }
        }
    }
</script>

<template>
    <h1>Task 6</h1>

    <textarea cols="30" rows="10" v-model="text7">Your texts</textarea>
    <p>{{text7}}</p>
</template>