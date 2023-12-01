<script>
import ChildComponent from './ChildComponent.vue';

    export default {
        methods: {
            func1: function() {
                alert("func1");
            },
            func2: function() {
                alert("func2");
            }
        },
        components: {
            ChildComponent
        }
    }
</script>

<template>
    <h1>Task 5</h1>

    <ChildComponent :func1="func1" :func2="func2" />
</template>