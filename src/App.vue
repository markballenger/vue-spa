<template>

<v-app dark toolbar>
  
  <header-bar ></header-bar>
  
  <v-container id="container" fluid fill-height>
    <v-layout>
      <v-flex xs6 offset-xs3>
        <router-view></router-view>
        <div class="help-text">
          <p>Vue.js 2 Single Page App (SPA) Example with vuex and vue-router.</p>
          <a href="https://github.com/skyronic/vue-spa">View Source Code</a>
        </div>
      </v-flex>
    </v-layout>
  </v-container>

  <v-footer fixed></v-footer>

</v-app>


</template>

<script>
import HeaderBar from '@/components/HeaderBar'
export default {
  components: {
    HeaderBar
  },
  name: 'app'
}
</script>

<style>
.help-text {
  margin-top: 20px;
  font-size: 12px;
}

/*
* adjust content for new vuetify toolbar
*/
#container{ 
  margin-top: 60px;
}
</style>
