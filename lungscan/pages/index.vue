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
      :continuous="false"
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
  </v-card>

<v-jumbotron color="grey lighten-2">
    <v-container fill-height>
      <v-layout align-center>
        <v-flex>
          <h3 class="display-3">Welcome to the site</h3>
          <span class="subheading">Lorem ipsum dolor sit amet, pri veniam forensibus id. Vis maluisset molestiae id, ad semper lobortis cum. At impetus detraxit incorrupte usu, repudiare assueverit ex eum, ne nam essent vocent admodum.</span>
          <v-divider class="my-3"></v-divider>
          <div class="title mb-3">Check out our newest features!</div>
          <v-btn large color="primary" class="mx-0">See more</v-btn>
        </v-flex>
      </v-layout>
    </v-container>
  </v-jumbotron>

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
            src: 'https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/s2048x2048/115966372_2679699138986444_5174549651740858420_n.jpg?_nc_cat=108&_nc_sid=b96e70&_nc_eui2=AeEINN5tQ_L4MSNxeElxJHCnUvERNeJu4XtS8RE14m7he0iY_AUGkOlZunetAIpZAufbS_wzMLiOfQJhNmNYkYOk&_nc_ohc=FHmJu9mB6UQAX_3Lu3m&_nc_ht=scontent.fbkk10-1.fna&_nc_tp=7&oh=27ec47d46d27228c90cf22d54fe12d01&oe=5F495E42',
          },
          {
            src: 'https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/s2048x2048/115990054_316499989719720_6355650263231465359_n.jpg?_nc_cat=110&_nc_sid=b96e70&_nc_eui2=AeHbTt0ZNF5OFxbgiUuaVPmQ_vviT0nrkwn---JPSeuTCaFD7Vllj1k28E9N7Yo7z4TJro33tuoWZ2pTy_XKuU-T&_nc_ohc=8n9fSf7RMdQAX9om0Mn&_nc_ht=scontent.fbkk10-1.fna&_nc_tp=7&oh=e30885f4588d6f79e874e73c47b26054&oe=5F480F6F',
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