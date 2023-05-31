<template>
    <div id="app">
        <table>
            <thead>
            <tr>
                <th>Price</th>
                <th>Time</th>
                <th>Name</th>
            </tr>
            </thead>
            <tbody>
            <tr v-for="item in data">
                <td>{{ item.Price }}</td>
                <td>{{ item.Time }}</td>
                <td>{{ item.Name }}</td>
            </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {
    name: "output"
}
</script>
<style scoped>

</style>