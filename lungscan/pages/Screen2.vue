<template>
<div >
<Nav />
<Footer/>

 <v-card  
   style="margin:auto"
    
    width="1000"
    height="650"
  >
    

    <v-toolbar
      color="#A32E2E"
      dark
      >
 
    <v-spacer />  <v-toolbar-title class="text-center"  ><h3  id="inspire" class="myFont">Result</h3></v-toolbar-title><v-spacer />
        
    </v-toolbar>

    <v-container fluid>
      <v-row dense >
       <v-card
   
    width="1500"
    height="500"
    outlined
  >
  <v-container fluid>
      <div align="center"
      justify="center">
     <v-img
      class="img-center"
      height="200px"
      width="200px"
      src="https://prod-images-static.radiopaedia.org/images/1436778/7c47ea1fb9a8510e765ef510d36012_jumbo.jpeg"
    >
      
    </v-img>

    
  
   
<v-jumbotron 
    
    color="grey lighten-2"
    align="center"
      justify="center" >
    <v-container fill-height>
      <v-layout align-center>
        <v-flex id="inspire" class="myFont">
          <h2 class id="inspire"   >Detect</h2>
          
        
          <h5 class="subheading">  </h5>
          <v-btn  rounded x-large color="#D93939"  class="mx-0" dark>Positive</v-btn>
        </v-flex>


        
      </v-layout>




    </v-container>
      <v-divider class="my-3"></v-divider>
  </v-jumbotron>


 <v-jumbotron 
    color="grey lighten-2"
    align="center"
      justify="center" >
    <v-container fill-height>
      
        <v-flex id="inspire" class="myFont">
          <h2 class id="inspire"   >Confident</h2>
          
        
          <h5 class="subheading">  </h5>
          <v-btn  rounded large   class="mx-0">Strong</v-btn>
          
        </v-flex>      
            
    </v-container>
  </v-jumbotron>
  
   




    </div>
<div align="center"
      justify="center" >
    <v-row >
 






<v-card-text id="inspire" class="myFont" >
  <h2 >
          ‘Emperical confirmation by specialist is required’
          </h2>
        </v-card-text>


</v-row>
</div>
   </v-container>
  
  </v-card >
  
      </v-row>
    </v-container>
<div align="center"
      justify="center" >
  
   <nuxt-link to="/Profile"> <v-btn x-large color="#478E00" id="inspire" class="myFont" >Record
      <v-icon dark right>mdi-checkbox-marked-circle</v-icon></v-btn></nuxt-link>
      <nuxt-link to="/Profile"> <v-btn x-large color="#A32E2E" id="inspire" class="myFont" >Discard<v-icon dark right>mdi-cancel</v-icon></v-btn></nuxt-link>
  
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

