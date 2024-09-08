<template>
  <div class="app">
    <div class="content">
      <router-view />
    </div>
  </div>
</template>

<style>
.app {
  position: relative;
  height: 100vh;
  margin: 0;
  background: #d7d7d7; /* Background color for the remaining part */

  overflow: auto; /* Ensure no overflow issues */
}

.content {
  position: relative;
  height: 100%;
  z-index: 2; /* Ensure this is above the background layer */
}

.app::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
    background: black; /* Background for the clipping path area */
  clip-path: polygon(50% 0, 100% 0, 100% 100%, 44% 100%);
  z-index: 1; /* Place this layer below the content */
}

.app::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: black; /* Background for the clipping path area */
  clip-path: polygon(55% 0, 100% 0, 100% 100%, 45% 100%);
  z-index: 0; /* Ensure this layer is above the background */
}
</style>
