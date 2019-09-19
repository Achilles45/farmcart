<template>
  <div class="home">
    <Navbar />
    <Banner />
    <Process />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Banner from "@/components/Banner.vue";
import Process from "@/components/Process.vue";

export default { 
  components:{
    Navbar,
    Banner,
    Process
  }
}
</script>
