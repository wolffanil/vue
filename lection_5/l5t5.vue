<script>
    export default {
        data() {
            return {
                text1: '',
                text2: '',
               
                    change: function() {
                        const text1 = this.text1;
                        this.text1 = this.text2;
                        this.text2 = text1;
                    }

            }
         
        }
    }

</script>s

<template>
    <h1>Task 5</h1>
    <input type="text" v-model="text1">
    <input type="text" v-model="text2">
    <button @click="change">Change input text</button>
</template>