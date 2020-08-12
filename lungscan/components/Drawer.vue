<template>
  <v-card
    id="inspire" class="myFont"
   
    color="grey lighten-4"
    flat
    height="200px"
    tile
  >
  
    <v-app-bar
      color="#A32E2E"
      dark
    >
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>

       <img src="../store/logo.png" width="30" height="30">
       

       <nuxt-link to="/Profile">  <v-btn text x-large color="primary" dark>Lungscan</v-btn></nuxt-link>

      <v-spacer></v-spacer>

   
  
   
    <nuxt-link to="/ProfileView"> <v-btn text large color="primary" dark >Profile</v-btn> </nuxt-link> 
    <nuxt-link to="/">  <v-btn text large color="primary" dark>Logout</v-btn></nuxt-link>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <nuxt-link to="/ProfileView"> <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
              
            </v-list-item-icon>
            <v-list-item-title>Profile</v-list-item-title>
          </v-list-item></nuxt-link>

            <nuxt-link to="/"> <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-arrow-left</v-icon>
            </v-list-item-icon>
           <v-list-item-title>Logout</v-list-item-title>
          </v-list-item></nuxt-link>

        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      drawer: false,
    }),
  }
</script>