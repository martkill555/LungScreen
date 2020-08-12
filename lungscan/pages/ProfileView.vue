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
      <h3  id="inspire" class="myFont" dark>Profile</h3>
      
   <v-spacer /> </v-card-title>
 <v-divider class="my-3"></v-divider>
 <v-container></v-container><v-container></v-container><v-container></v-container>
        <v-container>
      <v-img
      class="white--text align-end"
       height="250px"
      width="250px"
      src="https://scontent.fbkk22-1.fna.fbcdn.net/v/t1.0-9/p960x960/70286121_2507184436030743_4153033461684240384_o.jpg?_nc_cat=100&_nc_sid=85a577&_nc_eui2=AeFmHi3XXYNO64vAJFmkTg9eR9E0bJitpYlH0TRsmK2lidu8qt4yX6MjOsxZ_mefcktgaMuk5jmr6nLEGhJ4n8N8&_nc_ohc=SyOnbf2Rz6sAX84H2fN&_nc_ht=scontent.fbkk22-1.fna&_nc_tp=6&oh=f1f566c07a7fd282b0e71f62f7be01fe&oe=5F5B8D9D"
    >  </v-img>
<v-container></v-container>

<v-container>
  <nuxt-link to="/ProfileEdit"> <v-btn  x-large color="#D60000" id="inspire" class="myFont" dark>Edit Profile<v-icon dark right>mdi-wrench</v-icon></v-btn></nuxt-link>  
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
       <v-container></v-container><v-container></v-container><v-container></v-container><v-container></v-container><v-container></v-container>
    <v-row>
      <v-col cols="4">
        <v-card-text id="inspire" class="myFont"><h2>Name :</h2></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-card-text ><h3 id="inspire" class="myFont">Dr. Sarawut Rattanawichein</h3></v-card-text>
      </v-col>
    </v-row>
     <v-row>
      <v-col cols="4">
       <v-card-text id="inspire" class="myFont"><h2>Tel :</h2></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-card-text><h3 id="inspire" class="myFont">092-552-9166</h3></v-card-text>
      </v-col>
    </v-row><v-row>
      <v-col cols="4">
       <v-card-text id="inspire" class="myFont"><h2>Hospital :</h2></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-card-text ><h3 id="inspire" class="myFont">KMUTT Hospital</h3></v-card-text>
      </v-col>
       <v-col cols="4">
       <v-card-text id="inspire" class="myFont"><h2>Position :</h2></v-card-text>
      </v-col>
      <v-col cols="8">
        <v-card-text ><h3 id="inspire" class="myFont">Specialist</h3></v-card-text>
      </v-col>
       <v-container></v-container> <v-container> <v-divider class="my-3"></v-divider></v-container>
        <v-divider class="my-3"></v-divider>
       <v-card-text><h4 id="inspire" class="myFont">Lung Scan 2020</h4> </v-card-text>
    </v-row>
    
<v-container></v-container>
  

      
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

