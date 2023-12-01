<script>
    export default {
        data() {

            return {
                checked: false
            }
        }
    }

</script>

<template>
    <h1>Task 7</h1>

    <input type="checkbox" v-model="checked">
    <p v-if="checked">hEELO</p>
</template>