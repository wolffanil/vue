<script>
    export default {
        data() {
            return {
                text13: '',
                click13: function() {
                    if(this.text13 === '') return;
                    this.arr13.push(this.text13);
                    this.text13 = '';
                },
                arr13: []
            }

        }
    }
</script>

<template>
    <h1>Task 13</h1>
    <button @click="click13">btn</button>
    <input type="text" v-model="text13">

    <ul>
        <li v-for="item in arr13" :key="item">{{item}}</li>
    </ul>
    
</template>