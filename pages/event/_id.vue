<template>
  <div>
    <h1>Events #{{ id }}</h1>
  </div>
</template>
<script>
  export default {
    head() {
      return {
        title: `Event #${this.id}`,
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: `This is the event #${this.id}`,
          }
        ]
      }
    },
    computed: {
      id() {
        return this.$route.params.id
      },
    }
  }
</script>