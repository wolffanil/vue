<script>
    export default {
        props: {
            name: String,
            age: Number,
            salary: Number
        }
    }
</script>

<template>
    <li>
        <p>{{name}}</p>
        <p>{{age}}</p>
        <p>{{salary}}</p>

    </li>
</template>