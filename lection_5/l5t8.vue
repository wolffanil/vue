<script>
    export default {
        data() {
            return {
                arr8: []
            }
        }
    }
</script>

<template>
    <h1>task 8</h1>

    <ul>
        <li>
            <p>Russia</p>
            <input type="checkbox" v-model="arr8" value="russia">
        </li>

        <li>
            <p>German</p>
            <input type="checkbox" v-model="arr8" value="german">
        </li>

        <li>
            <p>Italia</p>
            <input type="checkbox" v-model="arr8" value="italia">
        </li>

    </ul>

    <p>{{arr8}}</p>
</template>