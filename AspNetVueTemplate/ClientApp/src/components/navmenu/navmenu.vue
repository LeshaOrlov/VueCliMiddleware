<template>
  <v-navigation-drawer app dark permanent>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="title">
            Vue.js
          </v-list-item-title>
          <v-list-item-subtitle>
            Template
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

        <v-divider></v-divider>
        <v-list
        dense
        nav
      >
        <v-list-item link to="/">
          <v-list-item-icon>
            <v-icon>mdi-home</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>



         <v-list-item link to="/counter">
          <v-list-item-icon>
            <v-icon>mdi-calculator</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Counter</v-list-item-title>
          </v-list-item-content>
        </v-list-item>



         <v-list-item link to="/fetchdata">
          <v-list-item-icon>
            <v-icon>mdi-table</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Fetch data</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

      </v-list>
     
  </v-navigation-drawer>
</template>


