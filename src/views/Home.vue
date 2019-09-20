<template>
  <div class="home">
    <Navbar />
    <Banner />
    <Process />
    <Farms />
    <Management />
    <CurrentNumbers />
    <Insurance />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Banner from "@/components/Banner.vue";
import Process from "@/components/Process.vue";
import Farms from "@/components/Farms.vue";
import Management from "@/components/Management.vue";
import CurrentNumbers from "@/components/CurrentNumbers.vue";
import Insurance from "@/components/Insurance.vue";
import Footer from "@/components/Footer.vue";

export default { 
  components:{
    Navbar,
    Banner,
    Process,
    Farms,
    Management,
    CurrentNumbers,
    Insurance,
    Footer
  }
}
</script>
