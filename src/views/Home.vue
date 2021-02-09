<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import OrderConfirm from "@/components/OrderConfirm.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    OrderConfirm,
  },
};
</script>
