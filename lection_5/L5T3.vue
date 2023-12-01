<script>


    export default { 
        data() {
            return {
                number1: 0,
                number2: 0,
                res: 0,
                calc: function() {
                    this.res = this.number1 + this.number2;
                }
            }
        }
    }
</script>

<template>
    <h1>Task 4</h1>
    <input type="number" v-model="number1">
    <input type="number" v-model="number2">
    <button v-on:click="calc">Calc</button>
    <p>{{res == 0 ? '' : res}}</p>   

</template>