<template>
  <div id="app" class="container">
    <div class="row">
      <div class="col-md-12">
        <h1>Usuarios</h1>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <TableUser :users="users"/>
      </div>
    </div>
  </div>
</template>

<script>
import TableUser from './components/TableUser.vue'

export default {
  name: 'App',
  components: {
    TableUser
  },
  data(){
    return{
      users: [
        {
          id: 1,
          nombre: 'Jon',
          apellido: 'Nieve',
          email: 'jon@email.com',
        },
        {
          id: 2,
          nombre: 'Tyrion',
          apellido: 'Lannister',
          email: 'tyrion@email.com',
        },
        {
          id: 3,
          nombre: 'Daenerys',
          apellido: 'Targaryen',
          email: 'daenerys@email.com',
        },
      ]
    }
  }
}
</script>

<style scoped>
  button {
    background: #009435;
    border: 1px solid #009435;
  }

</style>
