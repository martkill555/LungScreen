<template >
  <div style="background-image:url('https://cdn.discordapp.com/attachments/678634511214313493/737617401197232138/Main-BG.jpg'), background-repeat: no-repeat,
  background-size: auto">
  <NavBar/>
<div style="margin:auto" >
          <!-- <v-col cols="6" sm="3">
        <v-textarea
          label="Comment"
          auto-grow
          outlined
          rows="3"
          row-height="25"
          
        ></v-textarea>
          </v-col> -->
          <!-- <v-spacer></v-spacer> -->
          <!-- <v-jumbotron color="grey lighten-2" width="1500" height="1000">
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
  </v-jumbotron> -->
  <v-carousel>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>
</div>
<template>
 <v-parallax
    dark
    src='https://cdn.discordapp.com/attachments/678634511214313493/737617401197232138/Main-BG.jpg'
  >
    <v-row
      align="center"
      justify="center"
    >
      <v-col class="text-center" cols="12">
        <h1 class="display-1 font-weight-thin mb-4">MART</h1>
        <h4 class="subheading">xxxxxxxxxx</h4>
      </v-col>
    </v-row>
  </v-parallax>
</template>
  </div>
</template>
<style>
.bg {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background-image: "../store/Main-BG.jpg" width=25% height=25%;
    background-size: cover;
  }
</style>


<script>

import Navbar from '@/components/Nav'
 
export default ({data () {
      return {
        items: [
          {
            src: 'https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/74673290_1169269109937047_2053159281347264512_n.jpg?_nc_cat=101&_nc_sid=b96e70&_nc_eui2=AeEy_cjU33xmguVmC38v6I7m3yzAwQQzFWrfLMDBBDMVauKIVDgqS4Ni4AfqJ_lcWDIkSodAYphsoqcPb5liAjG1&_nc_ohc=JXLke9yrG2QAX9yD6my&_nc_ht=scontent.fbkk10-1.fna&oh=5542fa0340533f7cf759f12a6d370623&oe=5F49C897',
          },{
            src: 'https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/115991964_3909901282357773_5758477914104303027_n.jpg?_nc_cat=103&_nc_sid=b96e70&_nc_eui2=AeErbAf2NwQmSC2dpdm1ThjDtufZNV5t0Qi259k1Xm3RCBvBz4TXo2rZY-d5LCuXLVwhHnixvb1F1Bkxs4TrOwpM&_nc_ohc=5Y7X_RTOlZEAX_xIqyf&_nc_ht=scontent.fbkk10-1.fna&oh=444e22d63494b4265f6ec9f26c40e433&oe=5F469D51'
          },
          {
            src: 'https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/75521828_673109276551270_1502621173526036480_n.jpg?_nc_cat=101&_nc_sid=b96e70&_nc_eui2=AeHl49-Yxt3UqL07lU_-th1UB2eSgcl3uycHZ5KByXe7J6XMEcOd6ZeJsqaf-uKp-lzv2ly-40c2sDzRYxDh7jFS&_nc_ohc=7zYYiblDT-AAX_zurJj&_nc_ht=scontent.fbkk10-1.fna&oh=08764526fe40062a67515797d8179376&oe=5F477A4E'
          },
          {
            src: 'https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/90785475_555818048375458_3037732460386320384_n.jpg?_nc_cat=108&_nc_sid=b96e70&_nc_eui2=AeH4RzaWmmo4v3A88gdoss2sDc_lKpgOIMkNz-UqmA4gyQZ60FCa5qLjhSYscDRpljr883Jclh4BCCARVmrP0sKZ&_nc_ohc=baMSaF0-q14AX_x92yN&_nc_ht=scontent.fbkk10-1.fna&oh=cf66d09d54a80325e2b9db7047e0f50d&oe=5F469CAF'
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