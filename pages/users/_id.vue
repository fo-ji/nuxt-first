<template>
  <h1>username: {{ user.name }}</h1>
</template>

<script>
export default {
  data() {
    return {
      id: this.$route.params.id,
      users: [
        {
          id: 1,
          name: 'takeshi',
        },
        {
          id: 2,
          name: 'satoshi',
        },
        {
          id: 3,
          name: 'masashi',
        },
      ],
    }
  },
  computed: {
    user() {
      return this.users.find((user) => user.id == this.id)
    },
  },
}
</script>
