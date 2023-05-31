<script setup>

</script>

<template>
    <h1>Example: Shopping List</h1>
    <div id="app">
        <form v-on:submit.prevent="addItem">
            <p>
                What do you need?
                <input type="text" required placeholder="item name.." v-model="itemName">
            </p>
            <p>
                How many?
                <input type="number" placeholder="number of items.." v-model="itemNumber">
            </p>
            <button type="submit">Add item</button>
        </form>

        <div>
            <p>Shopping list:</p>
            <ul>
                <li v-for="item in shoppingList">{{ item.name }}, {{ item.number}}</li>
            </ul>
        </div>
    </div>
</template>

<style scoped>

</style>