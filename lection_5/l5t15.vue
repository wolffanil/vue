<script>
    export default {
        data() {
            return {
                users: [
			{
				id: 1,
				name: 'name1',
				salary: 100,
				age: 30,
			},
			{
				id: 2,
				name: 'name2',
				salary: 200,
				age: 40,
			},
			{
				id: 3,
				name: 'name3',
				salary: 300,
				age: 50,
			},
		],
		name: '',
				age: '',
				salary: '',
                removeUser: function(index) {
                    this.users = this.users.filter((item) => item.id !== index);
                },
                userId: '',

                editUser: function(id) {
                    this.userId = id;
					const user = this.users.filter((user) => user.id === id);
					
					this.name = user[0].name;
					this.age = user[0].age;
					this.salary = user[0].salary;
                },
			
				editData: function() {
					this.users = this.users.map((user) => {
						const currentuser = user.id === this.userId;
						if(currentuser) {
							user.name = this.name ? this.name : user.name;
							user.age = this.age ? this.age : user.age;
							user.salary = this.salary ? this.salary : user.salary;
							return user;
						} else {
							return user;
						}
					});

					this.userId = '';
					this.name = '';
					this.age = '';
					this.salary = '';
				}

            }

        }
    }
</script>

<template>
    <h1>Task 15</h1>
    

    <ul>
		<li v-for="user in users" :key="user.id">
			{{ user.name }}
			{{ user.age }}
            {{ user.salary }}

            <button @click="removeUser(user.id)">DeleteUser</button>
            <button @click="editUser(user.id)">Edit</button>
		</li>
	</ul>

    <div v-show="userId">
		<input type="text" v-model="name">
		<input type="number" v-model="age">
		<input type="number" v-model="salary">
		<button @click="editData">Edit</button>
    </div>


    
</template>