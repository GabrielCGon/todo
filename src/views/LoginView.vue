<template>
   <v-app id="inspire">
      <v-content>
         <v-container fluid fill-height>
            <v-layout align-center justify-center id="Visibilidade">
               <v-flex xs12 sm8 md4 >
                  <v-card class="elevation-12" >
                     <v-toolbar dark id="card" dense>
                        <v-toolbar-title id="logo">KJ すべて</v-toolbar-title>
                     </v-toolbar>
                     <v-card-text>
                        <v-form>                 
                           <v-text-field
                              shaped
                              outlined
                              prepend-icon="mdi-account"
                              name="login"
                              label="Email"
                              type="text"
                              
                           ></v-text-field>
                           <v-text-field
                              shaped
                              outlined
                              id="password"
                              prepend-icon="mdi-lock"
                              name="password"
                              label="Senha"
                              type="password"
                           ></v-text-field>                                         
                        </v-form>
                     </v-card-text>

                  </v-card>
               </v-flex>
            </v-layout>
         </v-container>
      </v-content>
   </v-app>
</template>
<script>
export default{

}

</script>
<style scoped>
  #card{
    display: flex;
    justify-content: space-around;
    background: linear-gradient(to left,#7E0F4B, #1A5865);

  }
  .container{
    background: linear-gradient(to right,#7E0F4B, #1A5865);
  }
  #Visibilidade{
    opacity: 1;
  }
  #logo{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    
  }

</style>