<template>
  <h1>
    This is specific page for specific user with id = {{ $route.params.id }}
  </h1>
</template>

<script>
export default {
    validate(data){
        return /^\d+$/.test(data.params.id);
    },
    layout: 'userlayout'
};
</script>

<style>
</style>