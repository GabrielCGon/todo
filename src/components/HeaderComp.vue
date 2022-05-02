<template>
  <v-card id="HeaderContainer"
    
  >
    <v-app-bar
      id="theme"
      dark
      tile
    >
      <v-app-bar-nav-icon @click="drawer = true" id="NavBtn"></v-app-bar-nav-icon>    
         <v-spacer></v-spacer>
      <v-item-group>       
        <v-btn      
          elevation="1"                 
          id="LoginBtn"
          to="/"
        >
          Sair
        </v-btn>     
      </v-item-group>
    
    </v-app-bar>
    <v-navigation-drawer 
      v-model="drawer"
      absolute
      temporary
      app
    >
      <v-list
        nav
        flat
      >
        <v-list-item-group
          v-model="group"
          active-class="primary--text text--accent-4"
        >
          <v-list-item to="">
            <v-list-item-icon>
              <v-icon>mdi-home-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Opção 1</v-list-item-title>
          </v-list-item>

          <v-list-item to="">
            <v-list-item-icon>
              <v-icon>mdi-home-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Opção 2</v-list-item-title>
          </v-list-item>

          <v-list-item to="">
            <v-list-item-icon>
              <v-icon>mdi-home-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Opção 3</v-list-item-title>
          </v-list-item>

          <v-list-item to="">
            <v-list-item-icon>
              <v-icon>mdi-home-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Opção 4</v-list-item-title>
          </v-list-item>

        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    <v-spacer></v-spacer>
  </v-card>
</template>

<script>
export default {
      data: () => ({
      drawer: false,
      group: null,
    }),
}
</script>

<style>
#HeaderContainer{
  width: 100%;
}

#LoginBtn{
  border: 1px solid white;
  background: linear-gradient(to right,#7E0F4B, #1A5865);
}

#theme{
  background: linear-gradient(to left,#606060, #343434, #868686);
}
#NavBtn{
  color: #ffffff;
  
}
</style>