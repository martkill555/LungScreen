<template>
<div >
<Nav />
<Footer/>

 <style>
.myFont {
  font-family:  Impact, Charcoal, sans-serif
}
</style>

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
    color="#A32E2E"
    dark
    width="500"
    height="600"
  >
    <v-card-title dark>
      
      <h3  id="inspire" class="myFont" dark>Manual Comment</h3>
      
    </v-card-title>
 <v-divider class="my-3"></v-divider>
 <v-row>
        
         <v-container>
       
      </v-container><v-container>
       
      </v-container>
      
          <v-card-text><h2 id="inspire" class="myFont"> Mr. Dhanyasit Ausavakulpairoj</h2> </v-card-text>
            
        
           <v-container>
       
      </v-container>
       
     
 </v-row>

    <v-list-item-title id="inspire" class="myFont">Program Detect</v-list-item-title>

   <v-col cols="12" sm="6" color="#A32E2E">
       
          <v-text-field dark
          id="inspire" class="myFont"
            v-model="first"
            label="Positive"
            solo
          ></v-text-field>
          
          
        </v-col>

         <v-list-item-title id="inspire" class="myFont">Confident</v-list-item-title>

   <v-col cols="12" sm="6" color="#A32E2E">
       
          <v-text-field dark
          id="inspire" class="myFont"
            v-model="first"
            label="Strong"
            solo
          ></v-text-field>
        </v-col>


   
      <v-container>
    
      </v-container>
      <v-container>
    
      </v-container>
      <v-container>
    
      </v-container>
       <v-divider class="my-3"></v-divider>
       <v-container>
    
      </v-container>
         <v-card-text><h4 id="inspire" class="myFont"> ID: 60130500213     Date: 20/10/62</h4> </v-card-text>
   
   
    
  </v-card>
   
     
    <v-card
    class="mx-auto"
     width="800"
    height="600"
  >
  <v-container>
    <v-img
      class="white--text align-end"
      height="180px"
      width="150px"
      src="https://prod-images-static.radiopaedia.org/images/1436778/7c47ea1fb9a8510e765ef510d36012_jumbo.jpeg"
    >
      <v-card-title></v-card-title>
    </v-img>
     <v-container>
    <v-list-item-title id="inspire" class="myFont" >Program Detect</v-list-item-title>
     <v-col class="d-flex" cols="12" sm="6">
        <v-select
        id="inspire" class="myFont" 
          :items1="items1"
          label="Abnormal"
          dense
        ></v-select>
      </v-col>

      <v-list-item-title id="inspire" class="myFont" >Confident</v-list-item-title>
     <v-col class="d-flex" cols="12" sm="6">
        <v-select
        id="inspire" class="myFont" 
          :items="items2"
          label="Strong"
          dense
        ></v-select>
      </v-col>

        <v-col cols="12" sm="6">
        <v-textarea
        id="inspire" class="myFont" 
          filled
          label="Note :"
          rows="2"
          row-height="10"
          
            
        ></v-textarea>
      </v-col>    
       <nuxt-link to="/Profile"> <v-btn  x-large color="#A32E2E" id="inspire" class="myFont" dark>Submit</v-btn></nuxt-link>  
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
      items1: ['Normal','Abnormal'],
      items2: ['Strong','Weakness'],
    }),
   
})
</script>