<script>
    export default {
        props: ['arg']
    }

</script>

<template>
    <h1>Task 3</h1>

    <ul>
        <li v-for="item in arg" :key="item">{{item}}</li>
    </ul>
</template>