<template>
  <div class="test">
    <h1>{{ title }}</h1>
    <p>{{ user.firstName }}</p>
    <p v-text="user.firstName"></p>
    <p v-if="showName">{{ user.lastName }}</p>
    <p v-else="showName">{{ user.firstName }}</p>

    <ul>
      <li v-for="item in items">{{ item.title }}</li>
    </ul>
    <button v-on:click="greet">Say Greeting</button>
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
      },
      showName: true,
      items: [
        { title: "Item One" },
        { title: "Item Two" },
        { title: "Item Three" }
      ]
    };
  },
  methods: {
    greet: function() {
      alert("Hello");
    }
  }
};
</script>

<style scoped></style>
