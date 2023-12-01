<script>


    export default { 
        data() {
            return {
                number: 0,
                res: 0,
                calc: function() {
                    this.res = this.number ** 2;
                }
                
            }
        }
    }

</script>

<template>
    <input type="number" v-model="number">
    <button v-on:click="calc">Calc</button>  
    <p>{{ res == 0 ? '': res}}</p>
</template>