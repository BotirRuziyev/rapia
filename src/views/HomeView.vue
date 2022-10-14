<template>
  <div class="home">
    <Home />
    <on-money />
  </div>
</template>

<script>
// @ is an alias to /src
import OnMoney from "@/components/OnMoney";
import Home from "@/components/Home";

export default {
  name: "HomeView",
  components: {
    OnMoney,
    Home,
  },
};
</script>
