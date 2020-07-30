<template>
<div >
<Nav />

   <v-card
    class="mx-auto"
    width="1600"
    height="1500"
    style="margin:auto"
  >
    

    <v-toolbar
      color="#A32E2E"
      dark
    >
     

      <v-toolbar-title>History</v-toolbar-title>

      <v-spacer></v-spacer>

      
    </v-toolbar>

    <v-container fluid>
      <v-row dense>
       <v-card
    class="mx-auto"
     width="1485"
     height="500"
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
     <v-text-field
        hide-details
        prepend-icon= mdi-magnify
         
        single-line
      ></v-text-field>
      <v-card flat>
    <v-card-text>
      <v-container fluid>
        <v-row>
          <v-col cols="12" sm="4" md="4">
            <v-checkbox
              v-model="ex4"
              label="ID"
              color="red"
              value="red"
              hide-details
            ></v-checkbox>
            <v-checkbox
              v-model="ex4"
              label="Date"
              color="red darken-3"
              value="red darken-3"
              hide-details
            ></v-checkbox>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-checkbox
              v-model="ex4"
              label="Detecable"
              color="indigo"
              value="indigo"
              hide-details
            ></v-checkbox>
            <v-checkbox
              v-model="ex4"
              label="Not Detectable"
              color="indigo darken-3"
              value="indigo darken-3"
              hide-details
            ></v-checkbox>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-checkbox
              v-model="ex4"
              label="Specialist"
              color="orange"
              value="orange"
              hide-details
            ></v-checkbox>
           
          </v-col>
        </v-row>

        <v-row class="mt-12">
          <v-col cols="12" sm="4" md="4">
            <v-checkbox
              v-model="ex4"
              label="Name"
              color="primary"
              value="primary"
              hide-details
            ></v-checkbox>
            <v-checkbox
              v-model="ex4"
              label="Last Name"
              color="secondary"
              value="secondary"
              hide-details
            ></v-checkbox>
          </v-col>
          <v-col cols="12" sm="4" md="4">
          
          </v-col>
          <v-col cols="12" sm="4" md="4">
           
           
          </v-col>
        </v-row>
      </v-container>
    </v-card-text>
  </v-card>
    </v-card-actions>
  <v-card
    class="mx-auto"
     width="1500"
    height="500"
  >
    <v-img
      class="white--text align-end"
       height="200px"
      width="200px"
      src="https://scontent.fbkk10-1.fna.fbcdn.net/v/t31.0-8/15440410_1164403710308829_709828196005354042_o.jpg?_nc_cat=110&_nc_sid=daf655&_nc_eui2=AeEYortViqWuVVOQ0iTeTh9SXkmtCFQlJmVeSa0IVCUmZUEWwuZ8FFckXAzl-RYnkRrqMkNh_uTvNk9Bvt-4tSvN&_nc_ohc=O4PDzAfYAVQAX9rdzA9&_nc_ht=scontent.fbkk10-1.fna&oh=bfe78e5534bc0e0716159342a5cbc329&oe=5F47B316"
    >
      <v-card-title></v-card-title>
    </v-img>

    <v-card-subtitle class="pb-0">28/07/2020</v-card-subtitle>

  <v-form>
    <v-container>
      <v-row>

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
            label="Case ID"
            outlined
          ></v-text-field>
        </v-col>
<v-col cols="6" sm="3">
        <v-textarea
          label="Detect"
          auto-grow
          outlined
          rows="3"
          row-height="25"
          
        ></v-textarea>
      </v-col>
      <v-col cols="6" sm="3">
        <v-textarea
          label="Comment"
          auto-grow
          outlined
          rows="3"
          row-height="25"
          
        ></v-textarea>
      </v-col>
      </v-row>
    </v-container>
  </v-form>
    </v-card-text>

    <v-card-actions>
      <nuxt-link to="/MoreInfo"> <v-btn x-large color="#EACB5E" dark>More Info</v-btn> </nuxt-link>

    <nuxt-link to="/Comment"> <v-btn x-large color="#A32E2E" dark>Manual Comment</v-btn> </nuxt-link>
    </v-card-actions>
  </v-card>
  <v-card
    class="mx-auto"
     width="1500"
    height="500"
  >
    <v-img
      class="white--text align-end"
       height="200px"
      width="200px"
      src="https://cdn.discordapp.com/attachments/678634511214313493/738322230781411378/106912103_144906173859246_4071149037015252191_n.png"
    >
      <v-card-title></v-card-title>
    </v-img>

    <v-card-subtitle class="pb-0">28/07/2020</v-card-subtitle>

  <v-form>
    <v-container>
      <v-row>

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
            label="Case ID"
            outlined
          ></v-text-field>
        </v-col>
<v-col cols="6" sm="3">
        <v-textarea
          label="Detect"
          auto-grow
          outlined
          rows="3"
          row-height="25"
          
        ></v-textarea>
      </v-col>
      <v-col cols="6" sm="3">
        <v-textarea
          label="Comment"
          auto-grow
          outlined
          rows="3"
          row-height="25"
          
        ></v-textarea>
      </v-col>
      </v-row>
    </v-container>
  </v-form>
    </v-card-text>

    <v-card-actions>
      <nuxt-link to="/MoreInfo"> <v-btn x-large color="#EACB5E" dark>More Info</v-btn> </nuxt-link>

    <nuxt-link to="/Comment"> <v-btn x-large color="#A32E2E" dark>Manual Comment</v-btn> </nuxt-link>
    </v-card-actions>
  </v-card>
  
  </v-card>
      </v-row>
    </v-container>
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
},
data: () => ({
      items: ['Staff','Specialist'],
    })
})
</script>

