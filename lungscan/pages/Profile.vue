<template>
<div >
<Nav />


     
<div>

 <v-layout>
   
    <v-flex xs12 sm6 offset-sm3>
      <v-card 
    max-width="1000"
    height="400">
        
       

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
        
<nuxt-link to="/ProfileEdit"> <v-btn x-large color="#A32E2E" dark>Edit Profile</v-btn> </nuxt-link>
       
      </v-card>
    </v-flex>
  </v-layout>
     <div class="my-2">

       
       <nuxt-link to="/Screen"> <v-btn x-large color="#3E6896" dark>Lung Screen</v-btn> </nuxt-link>
        
      </div>
      
    <v-col cols="12" sm="6">
        <div class="text-center">
          
          <div class="my-2">
            <nuxt-link to="/History"> <v-btn x-large color="#3E6896" dark>History</v-btn> </nuxt-link>
          </div>
        </div>
      </v-col>
      </div>
     
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
}
})
</script>

