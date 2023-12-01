<script>
  export default { 
    data() {
        return {
            choice: ''
        }
    }
  }
</script>

<template>
        <h1>Task 9</h1>

        <p>Russia</p>
        <input name="radio" type="radio" 
		v-model="choice" value="ru"> 
        <p>German</p>
	    <input name="radio" type="radio" 
		v-model="choice" value="ge"> 

        <p>Spanish</p>
	    <input name="radio" type="radio" 
		v-model="choice" value="sp"> 

        <p v-if="choice == 'ru'">Привет</p>
        <p v-if="choice == 'ge'">hello</p>
        <p v-if="choice == 'sp'">He</p>

</template>