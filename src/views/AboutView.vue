<template>
  <div class="about">
    <h1>This is an about page</h1>
    <HelloWorld msg="Welcome to Your Vue.js App" @update-ajah='doIncrement' />
    <p>nilai : {{ nilai }}</p>
  </div>
</template>

<script>
import HelloWorld from "../components/HelloWorld.vue";

export default {
  name: "AboutView",
  data() {
    return {
      nilai: 0,
    };
  },
  methods: {
    doIncrement() {
      this.nilai++;
    },
  },
  components: {
    HelloWorld,
  },
  /* mounted() {
    this.nilai++;
  }, */
};
</script>
