<template>
  <div>
    <div class="footer-main">
      <img
        class="pointer"
        src="../assets/ic_baseline-double-arrow.svg"
        alt=""
        @click="scrollToTop"
      />
      <div class="pointer usingnow-text" @click="scrollToTop">BACK TO TOP</div>
      <div
        class="social-icons mt-5 d-flex align-items-center justify-content-center"
      >
        <img class="pointer" src="../assets/Vector (4).svg" alt="linkedin" />
        <img class="ml-3 pointer" src="../assets/Vector (5).svg" alt="gmail" />
      </div>
      <div class="mt-5">@2024 NAYAK PAVANI</div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    scrollToTop() {
   this.$emit('scrollToTop')
    }
  }
};
</script>


<style scoped>
html {
  scroll-behavior: smooth;
}
.pointer {
  cursor: pointer;
}
.footer-main {
  background-color: black;
  color: white;
  padding: 1% 0;
  text-align: center;

  margin: 20px 0;

  width: 100%;
  box-sizing: border-box;
}
.usingnow-text {
  font-size: 1rem;
  font-weight: bold;
  letter-spacing: 3px;
}

.social-icons img.ml-3 {
  margin-left: 15px;
}
</style>
