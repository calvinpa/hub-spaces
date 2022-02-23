<template>
  <div class="about">
    <h1>This is an about page</h1>
    <profile></profile>
  </div>
</template>

<script>
import Profile from '../components/Profile.vue'
export default {
  name: 'About',

  components: {
    Profile
  }
}
</script>
