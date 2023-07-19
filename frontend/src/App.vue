<template>
  <router-view />
</template>

<script>
export default {
  data() {
  },
  mounted() {
  },
  methods: {
    logout() {
      this.$store.dispatch('logoutUser')
      .then(() => {
        this.$router.push({ name: 'Home' })
      })
    }
  }
 }
</script>

