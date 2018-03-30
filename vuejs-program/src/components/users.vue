/* eslint-disable */

<template>
  <div class="users">
    <h1>Users</h1>
  </div>
</template>

<script>
export default {
  name: 'users',
  data () {
    return {
     
    }
  },
  methods: {
    
  },
  mounted() {
    axios.get("'Authorization: Bearer KkiOCnOq2TVqtTZhhft24LW9zPQ7vwqwjp2jk6c1' http://api.wps-inc.com/products")
    .then(response => {this.results = response.data.results})
  }
}

</script>

<style scoped>

</style>
