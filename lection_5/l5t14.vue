<script>
    export default {
        data() {
            return {
                arr14: ['dff', 'bbb', 'ggg'],
                removeItem: function(index) {
                    this.arr14.splice(index, 1);



                }
            }

        }
    }
</script>

<template>
    <h1>Task 14</h1>
    

    <ul>
		<li v-for="(item, index) in arr14" :key="index">
			{{ item }}
			<button @click="removeItem(index)">remove</button>
		</li>
	</ul>

    
</template>