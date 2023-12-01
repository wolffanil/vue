<script>
    export default {
        data() {
            return {
                isDisabled: false,
                click12: function() {
                    this.isDisabled = !this.isDisabled;
                }
            }

        }
    }
</script>

<template>
    <h1>Task 12</h1>
    <button @click="click12">btn</button>
    <input type="text" :disabled="isDisabled">
    
</template>