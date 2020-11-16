<template>
  <v-app>
    <v-navigation-drawer
      app
      clipped
      permanent
      expand-on-hover
    >
      <!--  -->
    </v-navigation-drawer>
    <v-app-bar clipped-left style="-webkit-app-region: drag !important;" app color="light-blue accent-4" flat dark dense>
      <v-spacer></v-spacer>
      <v-btn
        icon
        style="-webkit-app-region: no-drag !important; z-index:1000;"
        @click="minimizeApp"
      >
      <v-icon size="14">mdi-window-minimize</v-icon>
      </v-btn>
      <v-btn
        icon
        style="-webkit-app-region: no-drag !important; z-index:1000;"
        @click="maximizeApp"
      >
      <v-icon size="14">mdi-window-maximize</v-icon>
      </v-btn>
      <v-btn
        icon
        style="-webkit-app-region: no-drag !important; z-index:1000;"
        @click="closeeApp"
      >
      <v-icon size="14">mdi-close</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <div  class="app-view">
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
      </div>
    </v-main>
  </v-app>
</template>

<script>
const { remote } = require('electron')
export default {
  name: "App",


  data: () => ({
  }),

  methods:{
    minimizeApp: () => {
      remote.BrowserWindow.getFocusedWindow().minimize()
    },
    maximizeApp: () => {
      remote.BrowserWindow.getFocusedWindow().maximize()
    },
    closeeApp:() => {
      remote.BrowserWindow.getFocusedWindow().close()
    }
  },

  created(){
    this.$vuetify.theme.dark = true
  }

};
</script>

<style lang="scss">
  html{
    overflow-y: hidden !important;
  }
  .app-view{
    overflow-y: auto !important;
    width: 100vw;
    height: calc(100vh - 48px);
  }
  /* width */
  ::-webkit-scrollbar {
    width: 10px;
  }

  /* Track */
  ::-webkit-scrollbar-track {
    background: transparent; 
  }
  
  /* Handle */
  ::-webkit-scrollbar-thumb {
    background: #0091EA; 
  }

  /* Handle on hover */
  ::-webkit-scrollbar-thumb:hover {
    background: #00B0FF; 
  }
</style>