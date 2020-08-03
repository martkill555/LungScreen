<template>
<div >
<Nav />
<Footer/>
<div>
       <v-row >
<!-- <v-col class="d-flex" cols="12" sm="6"> -->
<v-card
    class="mx-auto"
    max-width="400"
    style="margin-left:200px"
    outlined
   
  >
    <v-list-item three-line>
      <v-list-item-content>
        <div class="overline mb-4 mx-auto">Profile</div>
        <v-img src="https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/90785475_555818048375458_3037732460386320384_n.jpg?_nc_cat=108&_nc_sid=b96e70&_nc_eui2=AeH4RzaWmmo4v3A88gdoss2sDc_lKpgOIMkNz-UqmA4gyQZ60FCa5qLjhSYscDRpljr883Jclh4BCCARVmrP0sKZ&_nc_ohc=baMSaF0-q14AX_x92yN&_nc_ht=scontent.fbkk10-1.fna&oh=cf66d09d54a80325e2b9db7047e0f50d&oe=5F469CAF"></v-img>
        <v-list-item-title class="headline mb-1">Sarawut Rattanawichien</v-list-item-title>
        <v-list-item-subtitle>Dark Tall and Handsome</v-list-item-subtitle>
      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="80"
        color="grey"
      ></v-list-item-avatar>
    </v-list-item>

    <v-card-actions>
      <v-btn color="#A32E2E" @click="$refs.inputUpload.click()" dark>Select new image</v-btn>
<input v-show="false" ref="inputUpload" type="file" @change="yourFunction" >
    </v-card-actions>
  </v-card>
  <!-- </v-col > -->

    
      <v-col style="margin-left:300px" class="d-flex" cols="12" sm="6">
    <v-layout>
    <v-flex xs12 sm6 offset-sm3>
      <v-card
      max-width="700"
      >
        <v-card-title primary-title>
          <v-container>
      <v-row>

        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Name"
          ></v-text-field>
        </v-col>
       
        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Tel no."
          ></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Hospital"
          ></v-text-field>
        </v-col>

         <v-col class="d-flex" cols="12" sm="6">
        <v-select
          v-model="value"
          :items="items"
          label="Position"
          dense
        ></v-select>
      </v-col>

      </v-row>
    </v-container>
        </v-card-title>
        <div >
          <center>
<nuxt-link to="/Profile"> <v-btn x-large color="#A32E2E" dark>Save</v-btn> </nuxt-link>
          </center>
        </div>
      </v-card>
    </v-flex>
  </v-layout>
  </v-col>
    </v-row>
  
</div>

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
      value: ['Staff','Specialist'],
    })
})
</script>

