<template>
  <v-toolbar dense color="#A32E2E" >
     
        
    <img src="../store/logo.png" width="30" height="30">
       

      <v-btn text large color="primary" dark>Lungscan</v-btn>
  <v-spacer></v-spacer>
         
 <v-col cols="12" sm="2">
          <v-text-field
            v-model="last"
            label="Username"
            filled
            shaped
            dark=""
            
          ></v-text-field>
        </v-col>
       <v-col cols="12" sm="2">
          <v-text-field
            autocomplete="current-password"
            :value="userPassword"
            label="Password"
           
            :append-icon="value ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="() => (value = !value)"
            :type="value ? 'password' : 'text'"
            :rules="[rules.password]"
            @input="_=>userPassword=_"
            filled
            shaped
            dark=""
          ></v-text-field>
        </v-col>
  
    
    <nuxt-link to="/Profile">  <v-btn rounded color="#CC2E2E" dark>Login</v-btn></nuxt-link>
    
    </v-toolbar>

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