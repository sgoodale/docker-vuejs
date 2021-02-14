<template>
  <v-app>
    <v-card height="100%">

      <NavBar />

      <div class="mainContent">
        <v-main>
          <Main/>
        </v-main>
      </div>

    </v-card>
  </v-app>

</template>

<style>
  @import './stylesheets/layout.css';
</style>

<script>
import Main from './components/Main';
import NavBar from "./components/NavBar";

export default {
  name: 'App',

  components: {
    NavBar,
    Main,
  },

  data: () => ({
    //
  }),
};
</script>