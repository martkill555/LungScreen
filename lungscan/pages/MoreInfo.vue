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
    
    width="1000"
    height="650"
  >
    

    <v-toolbar
      color="#A32E2E"
      dark
      >
 
      <v-toolbar-title class="text-center"  ><h3  id="inspire" class="myFont">More Information</h3></v-toolbar-title>
      <v-spacer>  </v-spacer> 
        <v-toolbar-title class="text-center"  ><h5  >Case ID: 213</h5></v-toolbar-title>
    </v-toolbar>
 <v-container><v-row>
     <img
      height="50"
      width="50"
      src=" https://scontent.fbkk2-6.fna.fbcdn.net/v/t1.15752-9/116217099_295548811698040_8853209647408971802_n.png?_nc_cat=107&_nc_sid=b96e70&_nc_eui2=AeEbRPfShqaNql28UP0v7WOpoAFiJY2WL6egAWIljZYvp3jFgA1huAICdTEt0oZCzwI0dyp9wHwnsZnyUj1rnSdx&_nc_ohc=fKfd1KEVNYsAX8DkkW6&_nc_ht=scontent.fbkk2-6.fna&oh=7d2ac5e5c8db91738be28de343145023&oe=5F4C1B71"
    >
    
    <img
      height="150"
      width="150"
      src="https://prod-images-static.radiopaedia.org/images/1436778/7c47ea1fb9a8510e765ef510d36012_jumbo.jpeg"
    >
         <img
      height="50"
      width="50"
      src=" https://scontent.fbkk2-6.fna.fbcdn.net/v/t1.15752-9/116217099_295548811698040_8853209647408971802_n.png?_nc_cat=107&_nc_sid=b96e70&_nc_eui2=AeEbRPfShqaNql28UP0v7WOpoAFiJY2WL6egAWIljZYvp3jFgA1huAICdTEt0oZCzwI0dyp9wHwnsZnyUj1rnSdx&_nc_ohc=fKfd1KEVNYsAX8DkkW6&_nc_ht=scontent.fbkk2-6.fna&oh=7d2ac5e5c8db91738be28de343145023&oe=5F4C1B71"
    >
   <v-data-table style="margin:auto"
    
    :headers="headers3"
    :items="desserts3"
    
    hide-default-footer
    class="elevation-1"
  ></v-data-table>
      
      
    
 <v-spacer></v-spacer>
 <nuxt-link to="/Comment"> <v-btn rounded color="#A32E2E" id="inspire" class="myFont" dark>Manual Comment</v-btn></nuxt-link>
 </v-row>
</v-container>
<div> 
     <v-row>
  <v-card
    style="margin:auto"
    width="950"
    height="350"
    outlined
    shaped
  >
<v-container >
<v-row style="margin:auto">
   <v-card
    class="mx-auto"
    color="#EAEAEA"
    
    width="400"
  >
  <v-container>
   
    <v-card-title>
      
       <span  id="inspire" class="myFont">Program Detect</span>
    </v-card-title>
 
  <v-data-table style="margin:auto"
    
    :headers="headers"
    :items="desserts"
    
    hide-default-footer
    class="elevation-1"
  ></v-data-table>

    
 </v-container>
<v-container>
  </v-container>
    
  </v-card>
<v-spacer></v-spacer>
  <v-card
    class="mx-auto"
    color="#EAEAEA"
    
    width="500"
    height="320"
  >
    <v-container>
   
    <v-card-title>
      
       <span  id="inspire" class="myFont">Specialist Comment</span>
    </v-card-title>
 
  <v-data-table style="margin:auto"
    
    :headers="headers2"
    :items="desserts2"
    
    hide-default-footer
    class="elevation-1"
  ></v-data-table>

    
 </v-container>
<v-container>
  </v-container>
  </v-card>
  
</v-row>
</v-container>


 
  
  </v-card >
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
     data () {
      return {
        headers: [
          {
            text: 'Detect',
            align: 'start',
            value: 'name',
          },
          { text: 'Date', value: 'date' },
             
             ],
        desserts: [
          {
            name: 'Positive',
            date: '10/9/2020',             
                                
          },
          {
            name: 'Strong',
            date: '20/10/2020',             
                                
          },
          
              
        ],
        headers2: [
          {
            
            text: 'Comment',
            align: 'start',
            value: 'name',
          },
          { text: 'Description', value: 'description' }, 
          { text: 'Date', value: 'date' }, 
              
             ],
        desserts2: [
          {
            name: 'Positive',
            description: '-- --',
            date: '10/9/2020',             
                                
          },
          {
            name: 'Strong',
            description: '-- --',
            date: '20/10/2020',             
                                
          },
          
              
        ],
         headers3: [
          {
            text: 'Name',
            align: 'start',
            value: 'name',
          },
          { text: 'Date', value: 'date' }, 
          { text: 'Note', value: 'note' }, 
          
              
             ],
        desserts3: [
          {
            name: 'Mr. Dhanyasit Ausavakulpairoj',
            note: '-- --',
            date: '10/9/2020',             
                                
          },                  
              
        ],
      }
    },    
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

})
</script>

