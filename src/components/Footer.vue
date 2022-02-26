<template>
  <v-footer
    padless
  >
    <v-card
      class="flex"
      tile
    >
      <v-card-title class="justify-center">
        <v-btn
          v-for="sns in socials"
          :key="sns.icon"
          class="mx-4"
          icon
          :href="sns.href"
          target="_blank"
        >
          <v-icon size="24px" color="grey">
            {{ sns.icon }}
          </v-icon>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 --text text-center">
        {{ new Date().getFullYear() }} — <strong>{{profile.full_name}}</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
import profile from '../assets/profile.json'

export default {
  name: 'Footer',

  data: () => ({
    profile: profile,
    socials: [
      { icon: 'mdi-linkedin', href: 'https://www.linkedin.com/in/calvin-paulus' }
    ]
  })
}
</script>
