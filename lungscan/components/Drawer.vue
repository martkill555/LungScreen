<template>
  <v-card
    id="inspire" class="myFont"
   color="#AD2323"
    dark
    flat
    height="800"
    tile
    width="500"
  >
   <v-card-title dark>
<v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
    <img src="../store/logo.png" width="30" height="30"> <h3  id="inspire" class="myFont" >LUNGSCAN</h3>
    
    <v-spacer> </v-spacer>
     <nuxt-link to="/ProfileView"> <v-btn rounded color="#D60000" id="inspire" class="myFont" >View Profile</v-btn></nuxt-link>  
      
    </v-card-title>
 <v-divider class="my-3"></v-divider>
 <div  align="center"
      justify="center">
<v-container></v-container><v-container></v-container>

 <v-container>
   <v-img
      class="img-center"
      height="150px"
      width="150px"
      src="https://scontent.fbkk22-1.fna.fbcdn.net/v/t1.0-9/p960x960/70286121_2507184436030743_4153033461684240384_o.jpg?_nc_cat=100&_nc_sid=85a577&_nc_eui2=AeFmHi3XXYNO64vAJFmkTg9eR9E0bJitpYlH0TRsmK2lidu8qt4yX6MjOsxZ_mefcktgaMuk5jmr6nLEGhJ4n8N8&_nc_ohc=SyOnbf2Rz6sAX84H2fN&_nc_ht=scontent.fbkk22-1.fna&_nc_tp=6&oh=f1f566c07a7fd282b0e71f62f7be01fe&oe=5F5B8D9D"
    >
    
       </v-img> 
       <v-container></v-container>
       
       <v-container>
         
       <nuxt-link to="/Screen"> <v-btn  x-large color="#3E6896" id="inspire" class="myFont" >Lung Screen <v-icon  dark right>mdi-cloud-upload</v-icon></v-btn></nuxt-link>  
       
       
        </v-container>  
 </v-container>
 <nuxt-link to="/History"> <v-btn x-large color="#3E6896" id="inspire" class="myFont" >History</v-btn></nuxt-link>
 </div>
  
    <v-app-bar
      color="#AD2323"
      height="55"
      dark
    >
      
      

       
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      height="500"
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