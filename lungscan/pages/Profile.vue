<template>
<div >
<Nav />
<div >
 <!-- <v-layout >
    <v-flex xs12 sm6 offset-sm3>
      <v-card 
    max-width="1000"
    height="400"
     style="margin:auto">
        <v-card-title primary-title>Profile
          <v-container>
      <v-row>
        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Name"
          ></v-text-field>
        </v-col>
        <v-col cols="12" sm="6" md="3">
        <v-img src="../store/profile.jpg"></v-img>
        </v-col>
        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Tell"
          ></v-text-field>
        </v-col>
        <v-col cols="12" sm="6" md="3">
          <v-text-field
            label="Hospital"
          ></v-text-field>
        </v-col>

         <v-col class="d-flex" cols="12" sm="6">
        <v-select
          :items="items"
          label="Position"
          dense
        ></v-select>
      </v-col>

      </v-row>
    </v-container>
        </v-card-title>
        
<nuxt-link to="/ProfileEdit"> <v-btn x-large color="#A32E2E" dark>Edit Profile</v-btn> </nuxt-link>
       
      </v-card >
    </v-flex>
  </v-layout>
     <div class="my-2">

       
       <nuxt-link to="/Screen"> <v-btn x-large color="#3E6896" dark>Lung Screen</v-btn> </nuxt-link>
        
      </div>
      
    <v-col cols="12" sm="6">
        <div class="text-center">
          
          <div class="my-2">
            <nuxt-link to="/History"> <v-btn x-large color="#3E6896" dark>History</v-btn> </nuxt-link>
          </div>
        </div>
      </v-col>
      </div>
</div> -->
<v-row >
<v-col class="d-flex" cols="12" sm="6">
<v-card
    class="mx-auto"
    max-width="400"
    style="margin-left:200px"
    outlined
   
  >
    <v-list-item three-line>
      <v-list-item-content>
        <div class="overline mb-4 mx-auto">Profile</div>
        <v-img src="https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.0-9/16729224_1110358685756307_6038790989887994639_n.jpg?_nc_cat=109&_nc_sid=d4cf07&_nc_eui2=AeEn4EAotO8H1-3vH5XhYKWJdWQ5fAs5ngF1ZDl8CzmeAZ7mwZz9a_0JpDR8crPDbAl4GB1_aUYSJLYExKekf2kr&_nc_ohc=gIsgwmobf2MAX_Ccf-U&_nc_ht=scontent.fbkk10-1.fna&oh=6ec0f61d1ce95045c0c69a7d60072c40&oe=5F4626B3"></v-img>
        <v-list-item-title class="headline mb-1">Sarawut R.</v-list-item-title>
        <v-list-item-subtitle>Yed Master<br>Yed expert<br>agoda premium</v-list-item-subtitle>
      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="80"
        color="grey"
      ></v-list-item-avatar>
    </v-list-item>

    <v-card-actions>
     <nuxt-link to="/Screen"> <v-btn  color="#3E6896" dark>Lung Screen</v-btn></nuxt-link>
     <nuxt-link to="/History"> <v-btn  color="#A32E2E" dark>History</v-btn></nuxt-link>
    </v-card-actions>
  </v-card>
  </v-col >
  <v-col class="d-flex" cols="12" sm="6">
   <v-card
    class="mx-auto"
    max-width="700"
    
>
    <v-img
      src="https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/115991964_3909901282357773_5758477914104303027_n.jpg?_nc_cat=103&_nc_sid=b96e70&_nc_eui2=AeErbAf2NwQmSC2dpdm1ThjDtufZNV5t0Qi259k1Xm3RCBvBz4TXo2rZY-d5LCuXLVwhHnixvb1F1Bkxs4TrOwpM&_nc_ohc=5Y7X_RTOlZEAX_xIqyf&_nc_ht=scontent.fbkk10-1.fna&oh=444e22d63494b4265f6ec9f26c40e433&oe=5F469D51"
      height="200px"
    ></v-img>

    <v-card-title>
      Name : Sarawut Rattanawichien
    </v-card-title>
    <v-card-subtitle>
      Tel: 0925229196<br>
      Hospital: oyo 460 int place
  </v-card-subtitle>
    <v-card-actions>
      <nuxt-link to="/ProfileEdit"> <v-btn  color="#A32E2E" dark>Edit Profile</v-btn></nuxt-link>

      <v-spacer></v-spacer>

      <v-btn
        icon
        @click="show = !show"
      >
        <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <v-divider></v-divider>

        <v-card-text>
          Our goal is to save pussy.
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
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
}
})
</script>

