<template>
<div >
<Nav />


     

   <v-card
    class="mx-auto"
    width="1500"
    height="600"
  >
    

    <v-toolbar
      color="#A32E2E"
      dark
    >
     

      <v-toolbar-title>Case ID :</v-toolbar-title>

      <v-spacer></v-spacer>

      
    </v-toolbar>

    <v-container fluid>
      <v-row dense>
       <v-card
    class="mx-auto"
    width="1500"
    height="400"
    outlined
  >
    <!-- <v-list-item three-line>
      <v-list-item-content>
        <div class="overline mb-4">OVERLINE</div>
        <v-list-item-title class="headline mb-1">Headline 5</v-list-item-title>
        <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="80"
        color="grey"
      ></v-list-item-avatar>
    </v-list-item> -->

    <v-card-actions>
     
      <v-card flat>
    <v-card-text>
      
      <v-container fluid>
        <v-row>
          <v-img
      class="white--text align-end"
      height="200px"
      width="200px"
      src="https://scontent.fbkk2-5.fna.fbcdn.net/v/t31.0-8/p960x960/1506182_618107671602087_1288753790_o.jpg?_nc_cat=110&_nc_sid=7aed08&_nc_eui2=AeFmlqGqA6BAGGtEcKoCOdSxIHG_-CCmQ_wgcb_4IKZD_PKosA1i3Xn3WGpIEhMTW3zwTIOIFE5ImHLXysTuNZgm&_nc_ohc=IdUPWmZwkYMAX_2AWzQ&_nc_ht=scontent.fbkk2-5.fna&_nc_tp=6&oh=63b37d338d65b8633203ccc35f80fdbf&oe=5F454E22"
    >
      <v-card-title></v-card-title>
    </v-img>
          <v-col cols="6" sm="3">
          <v-text-field
            v-model="first"
            label="Name"
            outlined
          ></v-text-field>
        </v-col>

        <v-col cols="6" sm="3">
          <v-text-field
            v-model="last"
            label="Date"
            outlined
          ></v-text-field>
        </v-col>
 <v-col cols="6" sm="3">
          <v-text-field
            v-model="last"
            label="Note"
            outlined
          ></v-text-field>
        </v-col>
      <v-col cols="6" sm="3">
        <v-textarea
          label="Program Detect"
          auto-grow
          outlined
          rows="3"
          row-height="25"
          
        ></v-textarea>
      </v-col>
      <v-col cols="6" sm="3">
        <v-textarea
          label="Specialist Comment"
          auto-grow
          outlined
          rows="3"
          row-height="25"
          
        ></v-textarea>
      </v-col>
        </v-row>
      </v-container>
    </v-card-text>
  </v-card>
    </v-card-actions>
    
  
  
  </v-card>
  <nuxt-link to="/Comment"> <v-btn x-large color="#A32E2E" dark>Manual Comment</v-btn> </nuxt-link>
      </v-row>
    </v-container>
  </v-card>
     
 <template>
 <v-parallax
        src='https://cdn.discordapp.com/attachments/678634511214313493/737617401197232138/Main-BG.jpg'
  >
    
  </v-parallax>
</template>
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
    })
})
</script>

