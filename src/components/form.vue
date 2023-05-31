<script setup>

</script>

<template>
    <form v-on:submit.prevent="addItem">
        <label for="price">price</label>
        <input type="text" id="price" name="price" v-model="itemPrice">
        <label for="Time">Time</label>
        <input type="date" id="Time" name="Time" v-model="itemTime">
        <label for="name">name</label>
        <input type="text" id="name" name="name" v-model="itemName">
        <button type="submit">Submit</button>
    </form>
</template>
<script>
export default {
    data() {
        return {
            itemPrice: null,
            itemTime: null,
            itemName: null
        }
    },
    methods: {
        addItem(){
            let item = {
                time: this.itemTime,
                name: this.itemName,
                price: this.itemPrice
            }
            itemPrice: null
            itemTime: null
            itemName: null
        }
    }
}
</script>
<style scoped>

</style>