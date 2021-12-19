<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  /** @function validate whether param in a number  */
  validate(data) {
    return /^\d+$/.test(data.params.id);
  },
  layout: "users",
};
</script>
