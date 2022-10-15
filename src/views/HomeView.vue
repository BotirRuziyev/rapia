<template>
  <div class="home">
    <Home />
    <Deposit />
    <OnMoney />
    <Earnings/>
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import Home from "@/components/Home";
import Contact from "@/components/Contact";
import Deposit from '@/components/Deposit.vue';
import Earnings from '@/components/Earnings.vue';
import OnMoney from "@/components/OnMoney";
export default {
  name: "HomeView",
  components: {
    Deposit,
    Home,
    OnMoney,
    Earnings,
    Contact,
  },
};
</script>
