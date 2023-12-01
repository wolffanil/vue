<script>
    import User from './User.vue';

    export default {
       data() {
        return {
            users2: [
                {
                    id: 1,
                    name: 'Rishat',
                    age: 22,
                    salary: 334
                },
                {
                    id: 2,
                    name: 'Rishat2',
                    age: 3,
                    salary: 34
                },  {
                    id: 3,
                    name: 'Rishat3',
                    age: 224,
                    salary: 33
                },
            ]
        }
    },
    components: {
        User,
    }
    }

</script>

<template>
    <h1>Task 4</h1>

    <ul>
        <User
            v-for="user in users2"
            :key="user.id"
            :name="user.name"
            :age="user.age"
            :salary="user.salary"
        />
    </ul>
</template>