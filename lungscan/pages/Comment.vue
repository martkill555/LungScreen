<template>
<div >
<Nav />


     
<v-card
    class="mx-auto"
    color="#A32E2E"
    dark
    width="800"
    height="500"
  >
    <v-card-title>
      
      <span class="title font-weight-light">Manual Comment</span>
    </v-card-title>

    <v-list-item-title>Program Detect</v-list-item-title>

   <v-col cols="12" sm="6" color="#A32E2E">
       
          <v-text-field dark
            v-model="first"
            label="Positive"
            solo
          ></v-text-field>
        </v-col>

         <v-list-item-title>Confident</v-list-item-title>

   <v-col cols="12" sm="6" color="#A32E2E">
       
          <v-text-field dark
            v-model="first"
            label="Strong"
            solo
          ></v-text-field>
        </v-col>


    <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            src="https://scontent.fbkk2-5.fna.fbcdn.net/v/t31.0-8/p960x960/1506182_618107671602087_1288753790_o.jpg?_nc_cat=110&_nc_sid=7aed08&_nc_eui2=AeFmlqGqA6BAGGtEcKoCOdSxIHG_-CCmQ_wgcb_4IKZD_PKosA1i3Xn3WGpIEhMTW3zwTIOIFE5ImHLXysTuNZgm&_nc_ohc=IdUPWmZwkYMAX_2AWzQ&_nc_ht=scontent.fbkk2-5.fna&_nc_tp=6&oh=63b37d338d65b8633203ccc35f80fdbf&oe=5F454E22"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Dhanyasit A.</v-list-item-title>
        </v-list-item-content>

        <v-row
          align="center"
          justify="end"
        >
          
          <span class="subheading mr-2">ID :217</span>
          <span class="mr-1">·</span>
         
          <span class="subheading">29/07/2020</span>
        </v-row>
      </v-list-item>
    </v-card-actions>
  </v-card>
    <v-spacer>
        
    </v-spacer>
     
    <v-card
    class="mx-auto"
     width="800"
    height="600"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      width="200px"
      src="https://prod-images-static.radiopaedia.org/images/1436778/7c47ea1fb9a8510e765ef510d36012_jumbo.jpeg"
    >
      <v-card-title></v-card-title>
    </v-img>

    <v-list-item-title>Program Detect</v-list-item-title>
     <v-col class="d-flex" cols="12" sm="6">
        <v-select
          :items1="items1"
          label="Normal/Abnormal"
          dense
        ></v-select>
      </v-col>

      <v-list-item-title>Confident</v-list-item-title>
     <v-col class="d-flex" cols="12" sm="6">
        <v-select
          :items2="items2"
          label="Dectable"
          dense
        ></v-select>
      </v-col>
 <v-list-item class="grow">
        <v-col cols="12" sm="6">
        <v-textarea
         
          label="Note :"
          rows="4"
          row-height="30"
          
            
        ></v-textarea>
      </v-col>

        <v-row
          align="center"
          justify="end"
        >
          
          
          <span class="mr-1">·</span>
         
          <nuxt-link to="/Profile"> <v-btn x-large color="#A32E2E" dark>Submit</v-btn></nuxt-link>
        </v-row>
      </v-list-item>
    <v-card-actions>
     
     
    </v-card-actions>
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
      items1: ['Normal','Abnormal'],
    }),
    data: () => ({
      items2: ['Strong','Weakness'],
    })
})
</script>