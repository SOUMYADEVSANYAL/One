<template>
  <section class="container">
    <h1>This is the index page.</h1>
    <nuxt-link to="/users">Users</nuxt-link>
    <button @click="goToProducts">Products</button>
  </section>
</template>

<script>
export default {
  name: "IndexPage",
  methods:{
    goToProducts(){
      this.$router.push('/products')
    }
  }
};
</script>
