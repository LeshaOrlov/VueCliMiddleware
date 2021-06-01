<template>
  <v-app id="app-root">
    <MenuComponent />
    <v-main>
      <div class="content">
        <router-view></router-view>
      </div>
        
    </v-main>
  </v-app>
</template>

<script>
import navmenu from "./components/navmenu/navmenu";

export default {
  components: {
    MenuComponent: navmenu,
  },
};
</script>

<style scoped>
.content{
  padding: 32px!important;
}
</style>


