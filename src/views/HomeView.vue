<template>
  <div class="home">
    <on-money />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// @ is an alias to /src
import OnMoney from "@/components/OnMoney";

export default {
  name: "HomeView",
  components: {
    OnMoney,
  },
};
</script>
