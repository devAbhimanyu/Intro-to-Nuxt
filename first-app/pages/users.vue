<template>
  <div>
    <input v-model="userId" type="text" />
    <button @click="loadUser">Load</button>
    <nuxt-child />
  </div>
</template>
<script>
export default {
  layout: 'users',
  data() {
    return {
      userId: '',
    }
  },
  methods: {
    loadUser() {
      this.$router.push(`/users/${this.userId}`)
    },
  },
}
</script>
