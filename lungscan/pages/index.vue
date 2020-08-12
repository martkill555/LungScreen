<template >
  <div id="app">
  <NavBar/>
   <Footer/>
  
  <style>
.myFont {
  font-family:  maven pro
}

</style>
<div style="margin:auto" >
      
 <v-card style="margin:auto"
    elevation="24"
    max-width="2000"
    height="200"
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
    
    color="grey lighten-2"
    align="center"
      justify="center" >
    <v-container fill-height>
      <v-layout align-center>
        <v-flex id="inspire" class="myFont">
          <h1 class id="inspire"   >Tuberculosis screener</h1>
          
          <v-divider class="my-3"></v-divider>
          <h2 class="subheading">Lung Scan</h2>
          <v-btn large  color="#CC2E2E" dark class="mx-0">Discover Our Application</v-btn>
        </v-flex>


        
      </v-layout>


      
    </v-container>
  </v-jumbotron>
<div align="center"
      justify="center">
  <img src="https://scontent.fbkk2-5.fna.fbcdn.net/v/t1.15752-9/116080892_689019555014265_2885304354529837000_n.png?_nc_cat=110&_nc_sid=b96e70&_nc_eui2=AeFdTofX5j84Vd2jykt902M28IWWzNBD-7XwhZbM0EP7tUoHqi9cRg-m2n-cS_VSNzkS7d5ljYKVvlHa12uivsvA&_nc_ohc=Ci6ORpqZvAUAX_cxnBB&_nc_ht=scontent.fbkk2-5.fna&oh=503a91b244b8288686b749b1659b69b8&oe=5F493782"
   width="1000" height="200">
  </div>
  </v-card>



</div>




 

  <template>

</template>
  
  </div>
  
</template>




<script>

import Navbar from '@/components/Nav'
import Footer from '@/components/Footer'

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
  components: {
    Footer
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