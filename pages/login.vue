<template>
  <div>
    <v-btn @click="login">Login with Github</v-btn>
    <span v-if="$auth.$state.loggedIn">
      <p>Hello world</p>
    </span>
  </div>
</template>
<script>
  export default {
    methods: {
      login() {
        this.$auth.loginWith('github')
      }
    }
  }
</script>
