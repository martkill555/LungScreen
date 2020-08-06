<template>
<div  >
<Nav />
<Footer/>

         
  <v-card  
   style="margin:auto"
    
    width="1000"
    height="615"
  >
    

    <v-toolbar
      color="#A32E2E"
      dark
    >
     

     <v-spacer /> <v-toolbar-title  ><h3  id="inspire" class="myFont">Screen </h3></v-toolbar-title><v-spacer />

      

      
    </v-toolbar>

    <v-container fluid>
      <v-row dense >
       <v-card
   
    width="1500"
    height="450"
    outlined
  >
  <v-container fluid>
    <div align="center"
      justify="center">
     <v-img
      class="img-center"
      height="200px"
      width="200px"
      src="https://cdn.discordapp.com/attachments/678634511214313493/737600952722522133/logo.png"
    >
      
    </v-img>
    </div>
  <v-form >
    <v-container>
     <div align="center"
      justify="center" > 
 <v-btn rounded color="#FFFFFF" id="inspire" class="myFont" @click="$refs.inputUpload.click()" >Upload </v-btn>
<input v-show="false" ref="inputUpload" type="file" @change="yourFunction" >
        </div>

        <v-col cols="24" sm="15" md="20">
          <v-text-field
          id="inspire" class="myFont "
            v-model="Name"
            label="Name"
            >
            </v-text-field>

   <v-textarea
          label="Note"
           id="inspire" class="myFont "
          filled
          rows="3"
          row-height="25"
          
        ></v-textarea>

        </v-col>

       
      
    </v-container>
  </v-form>

    <v-row>
 

</v-row>
   </v-container>
  
  </v-card >
 
      </v-row>
    </v-container>
  <div align="center"
      justify="center">
     <nuxt-link to="/Screen2" > <v-btn x-large color="#A32E2E" dark id="inspire" class="myFont" >Submit</v-btn> </nuxt-link>
     </div>

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

