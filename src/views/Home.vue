<template>
  <div>
    <v-flex d-flex>
   <v-layout wrap class="mx-10">
       <v-flex md4 v-for="personaje in personajes" :key="personaje.id">
           <v-card class="card-container mt-8 mx-1 pb-2" max-width="500px" >
            <v-img :src="personaje.imagen" height="100px width:400px" class="ma-auto"></v-img>
            <v-card-title class="pt-3">{{ personaje.nombre }}</v-card-title>
          </v-card>
       </v-flex>
   </v-layout>
</v-flex>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
 data() {
   return {
     personajes: [
{
'id': 1,
'nombre': 'Morty',
'imagen': 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
},
{
'id': 2,
'nombre': 'Rick',
'imagen': 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
},
{
'id': 3,
'nombre': 'Summer',
'imagen': 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
},
{
'id': 4,
'nombre': 'Beth',
'imagen': 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
},
{
'id': 5,
'nombre': 'Jerry',
'imagen': 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
},
]
   }
 },
}
</script>
