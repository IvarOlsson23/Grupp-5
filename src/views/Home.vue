<template>
  <div class="home">
<<<<<<< HEAD
    <HelloWorld msg="Welcome to Your Vue.js App" />
=======
    <Cart />
>>>>>>> 7583d57ed62494bf013dcd10564afaff51d1af76
  </div>
</template>

<script>
<<<<<<< HEAD
  // @ is an alias to /src
<<<<<<< HEAD
  import HelloWorld from '@/components/HomePage.vue'
=======
  import Cart from '@/components/Cart.vue'
>>>>>>> 7583d57ed62494bf013dcd10564afaff51d1af76

  export default {
    name: 'Home',
    components: {
<<<<<<< HEAD
      HelloWorld
=======
      Cart
>>>>>>> 7583d57ed62494bf013dcd10564afaff51d1af76
    }
  }
=======
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
>>>>>>> 8a69d58f62c7e151608fbbe59b3b890b9469a0f3
</script>
