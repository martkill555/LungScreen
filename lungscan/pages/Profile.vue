<template>

<div >
 

 
<Footer/>
<Drawer/>
<v-container>
   <v-row>
<v-card
    class="mx-auto"
    color="#AD2323"
    dark
    width="500"
    height="500"
  >
    <v-card-title dark>
 
    <img src="../store/logo.png" width="30" height="30"> <h3  id="inspire" class="myFont" dark>LUNGSCAN</h3>
    
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
</v-card>

 <v-card
    
    width="1280"
    height="500"
    
  >
    <v-toolbar
      color="#AD2323"
      dark
    >
     

      <v-spacer /><v-toolbar-title id="inspire" class="myFont"><h2>History</h2></v-toolbar-title><v-spacer />

     

      
    </v-toolbar>

    <v-container fluid>
      

  <v-data-table
     
    :search="search"
    :headers="headers"
    :items="desserts"
    sort-by="calories"
    class="elevation-1"
  >
    <template v-slot:top >
      <v-toolbar flat color="white">
           <v-col cols="3">
         <v-text-field
        v-model="search"
        append-icon="mdi-magnify"
        label="Search"
        id="inspire" class="myFont"
        single-line
        hide-details
      ></v-text-field>
       </v-col>
        
        <v-spacer></v-spacer>
       
  
    <p>{{ selected }}</p>
    <v-checkbox v-model="selected" label="ID" value="John" id="inspire" class="myFont" ></v-checkbox>
    <v-checkbox v-model="selected" label="Date" value="Jacob" id="inspire" class="myFont"></v-checkbox>
     <v-checkbox v-model="selected" label="First Name" value="Jacob" id="inspire" class="myFont"></v-checkbox>
      <v-checkbox v-model="selected" label="Last Name" value="Jacob" id="inspire" class="myFont"></v-checkbox>
       <v-checkbox v-model="selected" label="Detectable" value="Jacob" id="inspire" class="myFont"></v-checkbox>
        <v-checkbox v-model="selected" label="Not Detectable" value="Jacob" id="inspire" class="myFont"></v-checkbox>
         <v-checkbox v-model="selected" label="Specialist" value="Jacob" id="inspire" class="myFont"></v-checkbox>
  
          
      </v-toolbar>
    </template >
    <template v-slot:item.actions="{ item }"  style="margin:auto">
      <nuxt-link to="/MoreInfo"> <v-btn  color="#EACB5E" dark id="inspire" class="myFont">More Info</v-btn></nuxt-link>
      <nuxt-link to="/Comment"> <v-btn  color="#A32E2E" dark id="inspire" class="myFont">Manual Comment <v-icon dark right>mdi-message-text</v-icon></v-btn></nuxt-link>
    
    </template>
  
  </v-data-table>

    
    
    </v-container>
  </v-card>

  </v-row>
  </v-container>


</div>

</template>

<script>

import Nav from '@/components/Nav'
 import Drawer from '@/components/Drawer'

export default ({

   data: () => ({
      drawer: false,
      group: null,
    }),

    watch: {
      group () {
        this.drawer = false
      },
    },
  
    computed: {
      bg () {
        return this.background ? 'https://cdn.vuetifyjs.com/images/backgrounds/bg-2.jpg' : undefined
      },
    },
  data () {
      return {
        selected: ['John'],
      }
    },
data: () => ({
  
      dialog: false,
      
       search: '',
      headers: [
        {
           
          text: 'Name',
          align: 'start',
          sortable: false,
          value: 'name',
        },
        { text: 'Case ID', value: 'caseID' },
        { text: 'Date', value: 'date' },
        { text: 'Detect', value: 'detect' },
        { text: 'Comment', value: 'comment' },
        { text: 'Actions', value: 'actions', sortable: false },
      ],
          
          }),
    
    watch: {
      dialog (val) {
        val || this.close()
      },
    },

    created () {
      this.initialize()
    },

    methods: {
      initialize () {
        this.desserts = [
          {
            name: 'Sarawut Rattanawichein',
            caseID: 60130500248,
            date: "20/10/2020",
            detect: 'Negative',
            comment: "-- --",
          },
          {
              name: 'Sarawut Rattanawichein',
            caseID: 60130500248,
            date: "20/10/2020",
            detect: 'Negative',
            comment: "-- --",
          },
          {
             name: 'Sarawut Rattanawichein',
            caseID: 60130500248,
            date: "20/10/2020",
            detect: 'Negative',
            comment: "-- --",
          },
           {
             name: 'Sarawut Rattanawichein',
            caseID: 60130500248,
            date: "20/10/2020",
            detect: 'Negative',
            comment: "-- --",
          },
           {
             name: 'Sarawut Rattanawichein',
            caseID: 60130500248,
            date: "20/10/2020",
            detect: 'Negative',
            comment: "-- --",
          },
          
        
      
        ]
      },

      editItem (item) {
        this.editedIndex = this.desserts.indexOf(item)
        this.editedItem = Object.assign({}, item)
        this.dialog = true
      },

      deleteItem (item) {
        const index = this.desserts.indexOf(item)
        confirm('Are you sure you want to delete this item?') && this.desserts.splice(index, 1)
      },

      close () {
        this.dialog = false
        this.$nextTick(() => {
          this.editedItem = Object.assign({}, this.defaultItem)
          this.editedIndex = -1
        })
      },

      save () {
        if (this.editedIndex > -1) {
          Object.assign(this.desserts[this.editedIndex], this.editedItem)
        } else {
          this.desserts.push(this.editedItem)
        }
        this.close()
      },
    },
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

