<template>
  <table class="table">
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">Nombre</th>
        <th scope="col">Apellido</th>
        <th scope="col">RUN</th>
        <th scope="col">Nacimiento</th>
        <th scope="col">edad</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(usuario, $index) of usuarios" :key="$index">
        <td>{{ $index }}</td>
        <td>{{ usuario.nombre }}</td>
        <td>{{ usuario.apellido }}</td>
        <td>{{ usuario.run }}</td>
        <td>{{ usuario.nacimiento }}</td>
        <td>{{ usuario.edad }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>

export default {
  name: 'App',
  data: () =>({
    usuarios : [
      {
        nombre: "jose",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      {
        nombre: "raul",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      {
        nombre: "pedro",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      {
        nombre: "maria",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      {
        nombre: "antonio",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      {
        nombre: "pepe",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      {
        nombre: "karen",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      {
        nombre: "constanza",
        apellido: "perez",
        run: "123456k",
        nacimiento: "12-04-67",
        edad: "12",
      },
      ]
    
  }),
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
