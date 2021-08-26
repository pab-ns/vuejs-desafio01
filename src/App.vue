<template>

<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">RUT</th>
      <th scope="col">Edad</th>
      <th scope="col">Fecha de Nacimiento</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(persona, $index) in personas" :key="$index">
      <td>{{$index}}</td>
      <td>{{persona.nombre}}</td>
      <td>{{persona.apellido}}</td>
      <td>{{persona.rut}}</td>
      <td>{{persona.edad}}</td>
      <td>{{persona.fechaNacimiento}}</td>
    </tr>
  </tbody>
</table>

</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data: () => ({
    personas: [
      {nombre: "Lionel", apellido: "Messi", rut:"1.234.567.8", edad: 30, fechaNacimiento: "16 Junio"},
      {nombre: "Juan Roman", apellido: "Riquelme", rut:"1.234.567.8", edad: 10, fechaNacimiento: "30 Agosto"},
      {nombre: "Pablo", apellido: "Arimar", rut:"1.234.567.8", edad: 16, fechaNacimiento: "24 Septiembre"},
      ]
  })

  // name: 'App',
  // components: {
  //   HelloWorld
  // }
}
</script>

<style>
</style>
