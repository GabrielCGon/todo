<template>
  <v-container fluid class="fill-height">
    <v-layout align-center justify-center>
      <v-flex xs12 sm8 md4>
        <v-card class="elevation-12">
          <v-toolbar color="secondary" dense> </v-toolbar>
          <v-card-text>
            <v-form>
              <v-text-field
                v-model="Email"
                name="login"
                label="Email"
                type="text"
                :rules="[rules.required, rules.counter, rules.email]"
              ></v-text-field>

              <v-text-field
                id="password"
                v-model="Password"
                name="password"
                label="Senha"
                type="password"
              ></v-text-field>
            </v-form>
          </v-card-text>
          <v-card-actions>
            <div id="SupportRouter">
              <router-link style="color: black" class="ma-2" id="routes" to=""
                >Esqueci minha senha</router-link
              >
              <router-link
                style="color: black"
                class="ma-2"
                id="routes"
                to="/cadastro_competidor"
                >Cadastre-se</router-link
              >
            </div>
            <v-spacer></v-spacer>
            <v-btn color="secondary" v-on:click="UserExist()">Entrar</v-btn>
              <v-alert
      transition="slide-y-transition"
      :value="Error"
      color="#2F323A"
      dark
      class="Error"
    >
      Email ou Senha incorreta!
    </v-alert>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>



  </v-container>
</template>

<script>
export default {



};
</script>

<style scoped>
#SupportRouter {
  font-size: smaller;
  text-decoration: underline;
}
.container {
  background-color: rgb(134, 63, 63);
  margin: 0 auto;
}
.Error{
  position: fixed;
  bottom: 1%;
}
.fade-enter-active {
  transition: opacity 3s ease-in-out;
}
.fade-enter-to {
  opacity: 1;
}
.fade-enter {
  opacity: 0;
}
</style>