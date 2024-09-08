<template>
  <div class="home">
    <div>
      <!-- <div class="w-50"> -->
        <Header />
        <MainBody />
      <!-- </div> -->
      <!-- <div class="w-50"> -->
      <!-- </div> -->
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import MainBody from "@/components/MainBody.vue";
import Header from "@/components/Header.vue";

export default {
  name: "Home",
  components: {
    MainBody,
    Header,
  },
};
</script>
<style scoped>
.home{
    /* display: flex; */
    /* flex-direction: row; */
    height: 100vh;


}
</style>
