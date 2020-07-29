<template>
<div>
  <NavBar />
  
<v-parallax
             <v-img src="https://cdn.discordapp.com/attachments/678634511214313493/737617401197232138/Main-BG.jpg" aspect-ratio="1.4"></v-img>
          >
</v-parallax>
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