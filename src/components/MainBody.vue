<template>
  <div>
    <div class="content">
      <div class="text-content">
        <span class="hai-text"> Hi,I am</span> <br />
        <span class="name-text">Nayak Pavani,</span> <br />
        <span class="developer-text">Front-end Developer</span><br />
        <div style="margin-top: 25px">
          <img src="../assets/git.svg" alt="''" />
          <img
            style="margin-left: 25px"
            src="../assets/linkedin.svg"
            alt="''"
          />
        </div>
      </div>
    </div>
    <div class="about-me">
      <div class="about-me-text">
        Hi there! I'm Nayak Pavani, a passionate front-end developer with 2 years
        of experience specializing in creating responsive and user-friendly web
        applications.<br/> I have a strong command of HTML, CSS, JavaScript, and
        Vue.js, with a focus on delivering clean, maintainable code. In addition
        to my technical expertise,<br/> I hold a Bachelor's degree in Computer
        Science and an MBA in Human Resources, giving me a unique perspective on
        both technology and team dynamics.
        <div class="readmore-text">
          READ MORE
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.readmore-text {
  position: relative;
  color: white;
  font-weight: bold;
  padding-top: 30px;
  padding-left: 15px;
  
}

.readmore-text::before,
.readmore-text::after {
  content: '';
  position: absolute;
  top: 28px; /* Position the line vertically */
  width: 2px; /* Thickness of the vertical line */
  height: 30px; /* Height of the line */
  background-color: white;
}

.readmore-text::before {
  left: 2px; /* Adjust this value to control the space between the text and left line */
}

.readmore-text::after {
  right: 90%; /* Adjust this value to control the space between the text and right line */
}

.about-me-text {
  color: white;
  font-size: 16px;
  margin-left: 10%;
  padding: 20px;
}
.about-me {
  background: black;
  margin-top: 8%;
}
.content {
  padding: 20px;
  margin-top: 13%;
  margin-left: 20%;
  margin-right: 20%;
}
.hai-text {
  font-style: Montserrat;
  font-size: 1.7rem; /* Larger font size for Pavani's Portfolio */
  color: black;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Drop shadow */
  font-weight: 600;
}
.name-text {
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
.developer-text {
  color: #909090;
  font-size: 1.5rem;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Drop shadow */
}
</style>
