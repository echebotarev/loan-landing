<template>
  <v-app>
    <v-app-bar app>
      <div class="mr-2">
        <v-img src="/images/logo.png" width="40" height="40" contain></v-img>
      </div>
      <v-toolbar-title v-text="title" />
    </v-app-bar>

    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    <v-footer app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      title: 'Кредит под залог квартиры',
    }
  },
}
</script>
