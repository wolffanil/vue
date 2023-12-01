<script>
export default { 
    data() {
        return {
            str: 'active volid'
        }
    }

}
</script>

<template>
    <h1>Task 2</h1>
    <p :class="str">text</p>
</template>