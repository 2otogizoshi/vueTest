<template>
  <div class="test">
    <h1>{{ title }}</h1>
    <p>{{ user.firstName }}</p>
    <p v-text="user.firstName"></p>
  </div>
</template>

<script>
export default {
  name: "test",
  data() {
    return {
      title: "Hello world",
      user: {
        firstName: "scott",
        lastName: "Iam"
      }
    };
  }
};
</script>

<style scoped></style>
