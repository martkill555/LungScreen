<template>
<div  align="center"
      justify="center"
       id="app">
   <style>
.myFont {
  font-family:  maven pro
}

</style>

<v-footer
    dark
    padless
    class="justify-center pl-0" inset app 
  >
    <v-card
      class="flex"
      flat
      tile
    >
      

      <v-card-text class="py-2 white--text text-center" >
       <strong >@2020 - Lungscan</strong>
      </v-card-text>
    </v-card>
  </v-footer>

  </div>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>