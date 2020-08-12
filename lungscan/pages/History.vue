<template>
<div >
<Nav />
<Footer/>
<div align="center"
      justify="center">
   <v-card
    
    width="1500"
    height="750"
    
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
    
})
</script>

