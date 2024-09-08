<template>
  <div class="content">
    <div class="text-content">
    <span class="hai-text">  Hi,I am</span> <br />
      <span class="name-text">Nayak Pavani,</span> <br />
      <span class="developer-text">Front-end Developer</span><br />
      <div style="margin-top: 25px;">
          <img src="../assets/git.svg" alt="''">
          <img style="margin-left:25px" src="../assets/linkedin.svg" alt="''">

    </div>

    </div>

  </div>
</template>

<script setup></script>

<style scoped>
.content {
padding: 20px;
margin-top: 20%;
}
.hai-text {
    font-style: Montserrat;
    font-size:1.7rem; /* Larger font size for Pavani's Portfolio */
    color: black;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Drop shadow */
    font-weight: 600;
}
.name-text{
    font-style: Montserrat;
    font-size: 2.5rem; /* Larger font size for Pavani's Name */
    color: black;
    font-weight: 700;
}
.text-content {
    text-align: left;
  font-size: 1.5rem; /* Adjust font size as needed */
  color: black; /* Text color */
  line-height: 1.6; /* Adjust line height for better readability */
}
.developer-text{
    color:#909090;
    font-size: 1.5rem;
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Drop shadow */
}
</style>
