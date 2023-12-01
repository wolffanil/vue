<script>
    export default {
        data() {
            return {
                selected5: 'Пн',
		        options: ['Пн', 'Вт', 'Ср', 'Чт', 'Пт', "Су", "Во"],

            }
        }
    }
</script>

<template>
    <h1>Task 11</h1>
    <select v-model="selected5">
		<option v-for="option in options" :key="option">{{ option }}</option>
	</select>
	
	<p>{{ selected5 }}</p>

</template>