<template>
  <div class="home">
    <Home />
    <on-money />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import OnMoney from "@/components/OnMoney";
import Home from "@/components/Home";
import Contact from "@/components/Contact";
export default {
  name: "HomeView",
  components: {
    OnMoney,
    Home,
    Contact,
  },
};
</script>
