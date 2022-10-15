<template>
  <div class="home">
    <Home />
<<<<<<< HEAD
    <on-money />
    <Contact />
=======
    <Deposit />
    <OnMoney />
>>>>>>> e866999830223cf399936465734fb24223080e06
  </div>
</template>

<script>
// @ is an alias to /src
import Home from "@/components/Home";
<<<<<<< HEAD
import Contact from "@/components/Contact";
=======
import Deposit from '@/components/Deposit.vue';
import OnMoney from "@/components/OnMoney";

>>>>>>> e866999830223cf399936465734fb24223080e06
export default {
  name: "HomeView",
  components: {
    Deposit,
    Home,
<<<<<<< HEAD
    Contact,
=======
    OnMoney,
>>>>>>> e866999830223cf399936465734fb24223080e06
  },
};
</script>
