<script>
    export default { 
        data() {
            return {
                setElement: function() {
                    this.styles = true;
                },
                styles: false
            }
        }
    }
</script>

<template>
    <h1>Task 4</h1>
  <button @click="setElement">Show elememt</button>

  <p :class="styles ? show: hiden">ELement</p>
  <p>{{styles}}</p>
</template>

<style>
</style>