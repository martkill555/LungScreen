<template>
<div >
<NavBar />
kuy rai sus 
<v-parallax
    dark
    src="../store/Main-BG.jpg"
  >
</v-parallax>
<div>
     
      </div>
</div>
</template>

<script>

import NavBar from '@/components/NavBar'
// export default {
//   components: {
//     Nav
//   }
// }
export default ({
  components: {
    NavBar
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

