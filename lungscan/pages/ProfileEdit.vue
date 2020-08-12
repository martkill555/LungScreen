<template>
<div >
<Nav />
<Footer/>
      


<v-card  
   style="margin:auto"
    
    width="1280"
    height="600"
  >
<div  align="center"
      justify="center">
  <v-row>   
<v-card
    class="mx-auto"
    color="#AD2323"
    dark
    width="500"
    height="600"
  >
    <v-card-title dark>
      <v-spacer />
      <h3  id="inspire" class="myFont" dark>Edit Profile</h3>
      
   <v-spacer /> </v-card-title>
 <v-divider class="my-3"></v-divider>
 <v-container></v-container><v-container></v-container><v-container></v-container>
        <v-container>
       <v-img
      class="img-center"
      height="200px"
      width="200px"
      src="https://cdn.discordapp.com/attachments/678634511214313493/737600952722522133/logo.png"
    >
       </v-img>
<v-container></v-container>

<v-container>
 <v-btn rounded x-large color="#3E6896" id="inspire" class="myFont" @click="$refs.inputUpload.click()" dark>Select new image <v-icon dark right>mdi-cloud-upload</v-icon></v-btn>
<input v-show="false" ref="inputUpload" type="file" @change="yourFunction" >
</v-container>
        </v-container>
     
 

   
   
   
    
  </v-card>
   
     
    <v-card
    class="mx-auto"
     width="800"
    height="600"
  >
  <v-container>
  
     <v-container>
       <v-container></v-container><v-container></v-container><v-container></v-container>
    <v-row>
      <v-col cols="4">
        <v-card-text id="inspire" class="myFont"><h3>Name :</h3></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-text-field id="inspire" class="myFont"
          label=""
          value="Dr. Sarawut Rattanawichein"
          prefix=": "
        ></v-text-field>
      </v-col>
    </v-row>
     <v-row>
      <v-col cols="4">
       <v-card-text id="inspire" class="myFont"><h3>Tel :</h3></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-text-field id="inspire" class="myFont"
          label=""
          value="092-552-9166"
          prefix=":"
        ></v-text-field>
      </v-col>
    </v-row><v-row>
      <v-col cols="4">
       <v-card-text id="inspire" class="myFont"><h3>Hospital :</h3></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-text-field id="inspire" class="myFont"
          label=""
          value="KMUTT Hospital"
          prefix=":"
        ></v-text-field>
      </v-col>
       <v-col cols="4">
       <v-card-text id="inspire" class="myFont"><h3>Position :</h3></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-select
        id="inspire" class="myFont" 
          :items="items"
          label="Specialist"
          
           
          
        ></v-select>
      </v-col>
    </v-row>
    
<v-container></v-container>
  

       <nuxt-link to="/Profile"> <v-btn  x-large color="#D60000" id="inspire" class="myFont" dark>Save</v-btn></nuxt-link>  
         </v-container>
         
        
      </v-container>
  </v-card>
  </v-row>
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
},
  data: () => ({
      items: ['Staff','Specialist'],
     
    }),
       
})
</script>

