<template >
  <div style="background-image:url('https://cdn.discordapp.com/attachments/678634511214313493/737617401197232138/Main-BG.jpg')">
  <NavBar/>
<div >
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
</div>
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
 
export default ({
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