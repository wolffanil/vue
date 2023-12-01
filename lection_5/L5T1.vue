<script>

    export default { 
        data() {
            return {
                message: ''
            }
        }
    }

</script>

<template>
    <h1>Task 1</h1>
    <input v-model="message">
	<p :class="uper">{{ message }}</p>
</template>

<style>
    p.uper {
        text-transform: uppercase;
    }
</style>