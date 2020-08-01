<template>



<div id="app">
  <style>
.myFont {
  font-family:  Impact, Charcoal, sans-serif
}
</style>
  <v-toolbar dense color="#A32E2E"  id="inspire" class="myFont">
     
        
    <img src="../store/logo.png" width="30" height="30">
       

    <v-btn text x-large color="primary" dark >Lungscan</v-btn>
  <v-spacer></v-spacer>
         
 <v-col cols="12" sm="2" >
           <v-text-field
            
          prepend-icon="mdi-account"
            autocomplete="current-username"
            :value="userUsername"
            label="Username"
             type="text"
            
            @click:append="() => (value = !value)"
            :type="value ? 'username' : 'text'"
            :rules="[rules.Username]"
            @input="_=>userUsername=_"
            filled
            =""
          ></v-text-field>
        </v-col>
       <v-col cols="12" sm="2">
          <v-text-field
          prepend-icon="mdi-lock"
            autocomplete="current-password"
            :value="userPassword"
            label="Password"
             type="text"
            :append-icon="value ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="() => (value = !value)"
            :type="value ? 'password' : 'text'"
            :rules="[rules.password]"
            @input="_=>userPassword=_"
            filled
            
            =""
          ></v-text-field>
        </v-col>
 
    
    <nuxt-link to="/Profile">  <v-btn large="" color="#CC2E2E" dark>Login</v-btn></nuxt-link>
    
    </v-toolbar>
    
</div>
</template>

<script>
  export default {
    data: () => ({
      userPassword: "",
      valid: true,
      value: true,
      rules: {
        required: value => !!value || "Required.",
        password: value => {
          const pattern = /^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#\$%\^&\*])(?=.{8,})/;
          return (
            pattern.test(value) ||
            ""
          );
        }
      }
    })
  };
</script>