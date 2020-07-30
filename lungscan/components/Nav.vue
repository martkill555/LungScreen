<template>
<v-card
     background-color="grey lighten-5"
    color="grey lighten-4"
    flat
    height="200px"
    tile
  >
    <v-toolbar dense color="#A32E2E" >
     
        
    <img src="../store/logo.png" width="30" height="30">
       

       <nuxt-link to="/Profile">  <v-btn text large color="primary" dark>Lungscan</v-btn></nuxt-link>

      <v-spacer></v-spacer>

   
  
   
    <nuxt-link to="/Profile"> <v-btn text large color="primary" dark>Profile</v-btn> </nuxt-link>
    <nuxt-link to="/">  <v-btn text large color="primary" dark>Logout</v-btn></nuxt-link>
    
      
    </v-btn>
    

    

     
    </v-toolbar>
  </v-card>
 
  </template>