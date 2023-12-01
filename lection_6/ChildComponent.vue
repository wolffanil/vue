<script>
    export default {
        props: {
            func1: {
                type: Function
            },
            func2: {
                type: Function
            }
        }
    }
</script>

<template>
    <button @click="func1">Func1</button>
    <button @click="func2">Func2</button>

</template>