<template>
  <div class="home">
    <Home />
    <on-money />
    <Contact />
    <Deposit />
    <OnMoney />
  </div>
</template>

<script>
// @ is an alias to /src
import Home from "@/components/Home";
import Contact from "@/components/Contact";
import Deposit from '@/components/Deposit.vue';
import OnMoney from "@/components/OnMoney";
export default {
  name: "HomeView",
  components: {
    Deposit,
    Home,
    Contact,
    OnMoney,
  },
};
</script>
