<template>
    <div id="table-user">
        <table class="table">
            <thead>
                <tr>
                <th>Nombre</th>
                <th>Apellido</th>
                <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="user in users" :key="user.id">
                    <td>{{ user.nombre }}</td>
                    <td>{{ user.apellido }}</td>
                    <td>{{ user.email }}</td>
                </tr>
            </tbody>

        </table>
    </div>
</template>

<script>
export default{
    name:'table-users',
    props:{
        users:Array
    }
}
</script>

<style scoped>

</style>
