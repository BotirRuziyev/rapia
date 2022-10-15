<template>
  <div id="app">
    <nav>
      <Header />
    </nav>
    <router-view />
    <nav>
      <Footer /> 
    </nav>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    Header,
    Footer,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Assistant:wght@200;300;400;500;600;700;800&family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Open+Sans:wght@300;400;500;600;700;800&family=Raleway:wght@100;200;300;400;500;600;700;800;900&family=Roboto:ital,wght@1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
@import url("https://fonts.googleapis.com/css2?family=Assistant:wght@200;300;400;500;600;700;800&family=Inter:wght@100;200;300;400;500;600;700;800;900&family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Raleway:wght@100;200;300;400;500;600;700;800;900&family=Roboto:ital,wght@1,100;1,300;1,400;1,500;1,700;1,900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Assistant:wght@200;300;400;500;600;700;800&family=Inter:wght@100;200;300;400;500;600;700;800;900&family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Open+Sans:wght@300;400;500;600;700;800&family=Raleway:wght@100;200;300;400;500;600;700;800;900&family=Roboto:ital,wght@1,100;1,300;1,400;1,500;1,700;1,900&display=swap");
#app {
  background: linear-gradient(90deg, rgba(238, 239, 241, 0.6) 14.45%, #FFFFFF 118.31%), linear-gradient(0deg, #E3E6E8, #E3E6E8), #FFFFFF;
}
</style>
