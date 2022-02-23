<template>
  <v-app>
    <v-app-bar
      app
      color="#cdcdcdd9"
      dark
      absolute
      shrink-on-scroll
      fade-img-on-scroll
      prominent
      scroll-target="#scrolling-techniques-3"
      src=".\assets\profile-banner.jpg"
    >
    <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(133, 133, 133, 0.8), rgba(25,32,72,.7)"
        ></v-img>
      </template>
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
    </v-app-bar>

    <v-main class="grey lighten-3">
      <v-container>
        <v-row>
          <v-col
            cols="12"
            sm="2"
          >
            <v-sheet
              rounded="lg"
              min-height="268"
            >
              <!--  -->
            </v-sheet>
          </v-col>

          <v-col
            cols="12"
            sm="8"
          >
            <v-sheet
              min-height="70vh"
              rounded="lg"
            >
              <router-view/>
            </v-sheet>
          </v-col>

          <v-col
            cols="12"
            sm="2"
          >
            <v-sheet
              rounded="lg"
              min-height="268"
            >
              <!--  -->
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  })
}
</script>
