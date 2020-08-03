<template>
<div >
<Nav />
<Footer/>
 <v-card
    class="mx-auto"
    max-width="800"
    height="690"
  >
    <v-img
      class="white--text align-end"
      height="300px"
      width="300px"
      src="https://prod-images-static.radiopaedia.org/images/1436778/7c47ea1fb9a8510e765ef510d36012_jumbo.jpeg"
    >
    
      <v-card-title >Result</v-card-title>
    </v-img>

    
      <v-col cols="4">
        <v-subheader>Detect</v-subheader>
      </v-col>
      <v-col cols="8">
        <v-text-field
          label="Positive/Negative"
          value=""
          prefix=":"
        ></v-text-field>
      </v-col>
       <v-col cols="4">
        <v-subheader>Confidence</v-subheader>
      </v-col>
      <v-col cols="8">
        <v-text-field
          label="Strong/Weak"
          value=""
          prefix=":"
        ></v-text-field>
      </v-col>
   

    <v-card-text class="text--primary">
      <div>‘Emperical confirmation by specialist is required’</div>

      
    </v-card-text>

    <v-card-actions>
      <nuxt-link to="/Profile"> <v-btn x-large color="#A32E2E" dark>Record</v-btn></nuxt-link>

      <nuxt-link to="/Profile"> <v-btn x-large color="#A32E2E" dark>Discard</v-btn></nuxt-link>
    </v-card-actions>
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
}
})
</script>

