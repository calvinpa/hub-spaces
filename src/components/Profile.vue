<template>
  <v-card elevation="6" outlined tile max-width="300">
      <v-card-title>
        <v-avatar size="56">
              <img
                alt="profile"
                :src="avatar_img"
              >
            </v-avatar><p class="ml-2 my-2">{{profile.full_name}}</p></v-card-title>
      <v-card-subtitle><p class="my-1">{{profile.fullname_ja}}</p></v-card-subtitle>
      <v-card-text>
        Email: {{profile.email}} <br>
        Contacts: {{profile.phone_number}}
      </v-card-text>
  </v-card>
</template>

<script>
import profile from '../assets/profile.json'

export default {
  name: 'Profile',
  data: () => ({
    profile: profile,
    avatar_img: require('../assets/avatar.jpg')
  })
}
</script>
