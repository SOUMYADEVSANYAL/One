<template>
  <section class="container">
    <h1>This is the user index page.</h1>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load users</button>
  </section>
</template>

<script>
export default {
  data() {
    return {
      userId: "",
    };
  },
  methods: {
    onLoadUser() {
      this.$router.push("/users/" + this.userId);
    },
  },
};
</script>
