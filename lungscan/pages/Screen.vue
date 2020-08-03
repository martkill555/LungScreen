<template>
<div >
<Nav />
<Footer/>


      <v-btn color="#A32E2E" @click="$refs.inputUpload.click()" dark>Upload</v-btn>
<input v-show="false" ref="inputUpload" type="file" @change="yourFunction" >
      
    <v-card
      class="mx-auto"
    max-width="1000"
    height="400"
  >
    <v-card-text>
      <div>Predict</div>
     
    </v-card-text>
    <v-card-actions>
       <v-col cols="12" sm="6">
        <v-textarea
         
          label="Name :"
          rows="1"
          row-height="30"
          
            
        ></v-textarea>
      </v-col>
       <v-col cols="12" sm="6">
        <v-textarea
         
          label="Note :"
          rows="4"
          row-height="30"
          
            
        ></v-textarea>
      </v-col>

    
     
    </v-card-actions>
    <v-card-actions>
      <nuxt-link to="/Screen2"> <v-btn x-large color="#A32E2E" dark>Submit</v-btn></nuxt-link>

      
    </v-card-actions>
  </v-card>
  
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

