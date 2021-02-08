<template>
  <div class="home">
    <Cart />
  </div>
</template>

<script>
// @ is an alias to /src
import Cart from "@/components/Cart.vue";

export default {
  name: "Home",
  components: {
    Cart
  }
};
</script>
