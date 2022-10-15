<template>
  <div class="home">
    <Home />
    <Deposit />
    <OnMoney />
  </div>
</template>

<script>
// @ is an alias to /src
import Home from "@/components/Home";
import Deposit from '@/components/Deposit.vue';
import OnMoney from "@/components/OnMoney";

export default {
  name: "HomeView",
  components: {
    Deposit,
    Home,
    OnMoney,
  },
};
</script>
