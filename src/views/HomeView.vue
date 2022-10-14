<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <on-money />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld";
import OnMoney from "@/components/OnMoney"

export default {
  name: "HomeView",
  components: {
    HelloWorld,
    OnMoney,
  },
};
</script>
