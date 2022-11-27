<template>
  <v-app id="inspire">
    <v-app-bar class="px-3" color="primary" flat density="compact">
      <v-avatar color="primary" size="32" icon="mdi-vuetify"></v-avatar>

      <v-spacer></v-spacer>
      <v-tabs centered color="secondary">
        <v-tab v-for="link in links" :key="link">
          {{ link }}
        </v-tab>
      </v-tabs>
      <v-spacer></v-spacer>

      <v-avatar
        class="hidden-sm-and-down"
        color="other"
        size="32"
        icon="mdi-vuetify"
      ></v-avatar>
    </v-app-bar>

    <v-main class="bg-secondary">
      <v-container>
        <v-row>
          <v-col cols="12" sm="2">
            <v-sheet rounded="lg" color="use" min-height="50vh">

            </v-sheet>
          </v-col>

          <v-col cols="12" sm="8">
            <v-sheet min-height="70vh" color="use" rounded="lg">
            </v-sheet>
          </v-col>

          <v-col cols="12" sm="2">
            <v-sheet rounded="lg" color="use" min-height="20vh">
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script lang="ts">
export default {
  data: () => ({
    links: ["Dashboard", "Messages", "Profile", "Updates"],
  }),
};
</script>
