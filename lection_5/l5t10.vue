<script>
    export default {
        data() {
            return {
                city: ''
            }
        }
    }
</script>

<template>
    <h1>Task 10</h1>

    <select v-model="city">
		<option>Астрахань</option>
		<option>Волгоград</option>
		<option>Москва</option>
	</select>
	
	<p>{{ city }}</p>

</template>