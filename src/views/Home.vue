<template>
  <div class="home">
    <div>
      <MainBody />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import MainBody from "@/components/MainBody.vue";

export default {
  name: "Home",
  components: {
    MainBody,
  },
};
</script>
<style scoped>
.home {
  height: 100vh;
}
</style>
