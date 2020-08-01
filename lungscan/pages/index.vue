<template >
  <div style="background-image:url('https://cdn.discordapp.com/attachments/678634511214313493/737617401197232138/Main-BG.jpg'), background-repeat: no-repeat,
  background-size: auto">
  <NavBar/>
<div style="margin:auto" >
      
 <v-card style="margin:auto"
    elevation="24"
    max-width="2000"
    
    class="mx-auto"
  >
    
    <v-carousel
     
      cycle
      :show-arrows="false"
      hide-delimiter-background
      delimiter-icon="mdi-minus"
      height="300"
    >
      <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
    </v-carousel>
    <v-list two-line>
  
        
    </v-list>

    <v-jumbotron 
    
    color="grey lighten-2" >
    <v-container fill-height>
      <v-layout align-center>
        <v-flex >
          <h1 class id="inspire"   >Discover Our Application</h1>
          <span class="subheading">Lungscan</span>
          <v-divider class="my-3"></v-divider>
          <div class="title mb-3">Tuberculosis screener!</div>
          <v-btn large  color="#CC2E2E"dark class="mx-0">See more</v-btn>
        </v-flex>
      </v-layout>
    </v-container>
  </v-jumbotron>
  </v-card>



</div>
<template>
 <v-parallax
        src='https://cdn.discordapp.com/attachments/678634511214313493/737617401197232138/Main-BG.jpg'
  >
    
  </v-parallax>
</template>




  </div>
</template>



<script>

import Navbar from '@/components/Nav'
 
export default ({data () {
      return {
        items: [
          {
            src: 'https://scontent.fbkk2-8.fna.fbcdn.net/v/t1.15752-9/s2048x2048/116155080_296439891457897_1691392196203392050_n.jpg?_nc_cat=100&_nc_sid=b96e70&_nc_eui2=AeG7xisKlr15KFeP43WImX2TlQhsj8xqxfWVCGyPzGrF9Q_LWW5s_eFWNB04BxETI8pu5WATJ0jIDZPiqB673JPn&_nc_ohc=W6uYixZQwxMAX-LIGX6&_nc_ht=scontent.fbkk2-8.fna&_nc_tp=7&oh=28cee62d948413c57f694076a8b6377e&oe=5F4BBB66',
          },
          {
            src: 'https://scontent.fbkk2-8.fna.fbcdn.net/v/t1.15752-9/s2048x2048/116058418_632745694315024_1285163407543643633_n.jpg?_nc_cat=103&_nc_sid=b96e70&_nc_eui2=AeGeaB9Ksi-YYlboGExzIf-6j7mCn6Qma_iPuYKfpCZr-NfJ2125nqUedvKiYJ4yMwFBgMArf1NYDzb61f1-zryR&_nc_ohc=cr-_BPeLz10AX9y9hZ5&_nc_ht=scontent.fbkk2-8.fna&_nc_tp=7&oh=9a92501b7a1f15cd5aa97658651ccfdd&oe=5F4A8D0F',
          },
         
        ],
      }
    },
  components: {
    Navbar
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