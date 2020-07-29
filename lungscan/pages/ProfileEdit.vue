<template>
<div >
<Nav />


     

    <v-btn color="#A32E2E" @click="$refs.inputUpload.click()" dark>Select new image</v-btn>
<input v-show="false" ref="inputUpload" type="file" @change="yourFunction" >
      
    <v-layout>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
       

        <v-card-title primary-title>
          <v-container>
      <v-row>

        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Name"
          ></v-text-field>
        </v-col>
       
        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Tell"
          ></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Hospital"
          ></v-text-field>
        </v-col>

         <v-col class="d-flex" cols="12" sm="6">
        <v-select
          :items="items"
          label="Position"
          dense
        ></v-select>
      </v-col>

      </v-row>
    </v-container>
        </v-card-title>
        
<nuxt-link to="/Profile"> <v-btn x-large color="#A32E2E" dark>Save</v-btn> </nuxt-link>
       
      </v-card>
    </v-flex>
  </v-layout>
     
 
</div>
  

</template>

<script>

import Nav from '@/components/Nav'
// export default {
//   components: {
//     Nav
//   }
// }
export default ({
    
  components: {
    Nav
  },
  head () {
    
    return {
      script: [
        { src: 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js' }
      ],
      link: [
        { rel: 'stylesheet', href:'https://fonts.googleapis.com/css2?family=Maven+Pro:wght@800&display=swap' }
      ]
    }
},
data: () => ({
      items: ['Staff','Specialist'],
    })
})
</script>

