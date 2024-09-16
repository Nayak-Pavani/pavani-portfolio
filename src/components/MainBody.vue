<template>
  <div>
    <Header id="main-content" @scroll-to-section="scrollToSection" />
    <div>
      <div class="profile-page">
        <div class="content">
          <div class="d-flex justify-content-between align-items-center">
            <div class="text-content">
              <span class="hai-text"> Hi, I am</span> <br />
              <span class="name-text">Nayak Pavani,</span> <br />
              <span class="developer-text">Front-end Developer</span> <br />
              <div class="social-icons mt-3">
                <img
                  class="pointer"
                  @click="gitRepo()"
                  src="../assets/git.svg"
                  alt="GitHub"
                />
                <img
                  @click="linkedin()"
                  class="ml-3 pointer"
                  src="../assets/linkedin.svg"
                  alt="LinkedIn"
                />
                <a href="mailto:nayakpavani676@gmail.com">
                  <img
                    class="ml-3 pointer"
                    src="../assets/gmail.svg"
                    alt="gmail"
                  />
                </a>
              </div>
            </div>

            <!-- Profile Image on the Right -->
            <!-- <div class="profile-image">
          <img src="../assets/profile.png" alt="Profile" />
        </div> -->
          </div>
        </div>

        <!-- About Me Section: Positioned at the bottom -->
        <div class="about-me">
          <div class="about-me-text">
            Hi there! I'm Nayak Pavani, a passionate front-end developer with 2
            years of experience specializing in creating responsive and
            user-friendly web applications.<br />
            I have a strong command of HTML, CSS, JavaScript, and Vue.js, with a
            focus on delivering clean, maintainable code. In addition to my
            technical expertise, I hold <br />a Bachelor's degree in Computer
            Science and an MBA in Human Resources, giving me a unique
            perspective on technology and team dynamics.
            <div class="readmore-text mt-4">
              <img class="line-svg-left" src="../assets/Line.svg" alt="" />
              <span class="line-svg-right" 
                >READ MORE</span
              >
              <img class="line-svg-right" src="../assets/Line.svg" alt="" />
            </div>
          </div>
        </div>
        <div class="radial-background">
          <div id="about-me">
            <div
              class="d-flex align-items-center justify-content-center"
              style="margin-top: 30%"
              
            >
              <div class="about-me-box">ABOUT ME</div>
            </div>

            <!-- Additional Content after "ABOUT ME" box -->
            <div
            
              class="extra-content mt-4 d-flex align-items-center justify-content-center"
            >
              <p>
                I'm passionate about continuous learning and growing in the tech
                industry.I enjoy exploring new technologies and working on
                personal projects.<br />

                To know more about my educational qualification and work
                experience,
                <a :href="linkedinLink" target="_blank" class="linkedin-link"
                  >Click here</a
                >.
              </p>
            </div>
          </div>

          <div
            class="d-flex align-items-center justify-content-center"
            style="margin-top: 3%"
          >
            <img class="line-svg" src="../assets/black-line.svg" alt="" />
            <span class="explore-text" @click="toggleReadMore">Explore</span>
            <img class="line-svg" src="../assets/black-line.svg" alt="" />
          </div>
          <div
            class="d-flex align-items-center justify-content-center"
            style="margin-top: 3%"
          >
            <img class="line-svg" src="../assets/separatorBlack 1.svg" alt="" />
          </div>
          <div id="skills">
            <div
              class="d-flex align-items-center justify-content-center"
              style="margin-top: 3%"
            >
              <div class="about-me-box">Skills</div>
            </div>
            <div>
              <div
                class="usingnow-text"
                style="margin-left: 27%; margin-top: 3%"
              >
                USING NOW
              </div>
              <div
                class="d-flex align-items-center justify-content-between"
                style="margin-left: 27%; margin-top: 3%; margin-right: 27%"
              >
                <div class="icon-container icon1">
                  <img src="../assets/HTML.svg" alt="HTML" />
                  <div class="icon-name mt-3">HTML</div>
                </div>
                <div class="icon-container icon2">
                  <img src="../assets/CSS3.svg" alt="CSS3" />
                  <div class="icon-name mt-3">CSS3</div>
                </div>
                <div class="icon-container icon3">
                  <img src="../assets/JS.svg" alt="JavaScript" />
                  <div class="icon-name mt-3">JAVASCRIPT</div>
                </div>
                <div class="icon-container icon4">
                  <img src="../assets/JS.svg" alt="JavaScript" />
                  <div class="icon-name mt-3">JAVASCRIPT</div>
                </div>
              </div>
              <div
                class="d-flex align-items-center justify-content-between"
                style="margin-left: 25%; margin-top: 3%; margin-right: 28%"
              >
                <div class="icon-container icon5">
                  <img src="../assets/bootstrap.svg" alt="HTML" />
                  <div class="icon-name mt-3">BOOTSRAP</div>
                </div>
                <div class="icon-container icon6 ">
                  <img src="../assets/figma.svg" alt="CSS3" />
                  <div class="icon-name mt-3">FIGMA</div>
                </div>
                <div class="icon-container icon7">
                  <img src="../assets/git2.svg" alt="JavaScript" />
                  <div class="icon-name mt-3">GIT</div>
                </div>
                <div class="icon-container icon8">
                  <img src="../assets/React.svg" alt="JavaScript" />
                  <div class="icon-name mt-3">React</div>
                </div>
              </div>
            </div>
            <div>
              <div
                class="usingnow-text"
                style="margin-left: 27%; margin-top: 3%"
              >
                LEARNING
              </div>
              <div
                class="d-flex align-items-center justify-content-between"
                style="margin-left: 27%; margin-top: 3%; margin-right: 27%"
              >
                <div class="icon-container icon9">
                  <img src="../assets/mongodb.svg" alt="HTML" />
                  <div class="icon-name mt-3">MONGO DB</div>
                </div>
                <div class="icon-container icon10">
                  <img src="../assets/Nodejs.svg" alt="CSS3" />
                  <div class="icon-name mt-3">NODE JS</div>
                </div>
                <div class="icon-container icon11">
                  <img src="../assets/TypeScript.svg" alt="JavaScript" />
                  <div class="icon-name mt-3">TYPESCRIPT</div>
                </div>
              </div>
            </div>
          </div>
          <div id="contact-me">
            <div
              class="d-flex align-items-center justify-content-center"
              style="margin-top: 5%"
            >
              <div class="about-me-box">CONTACT ME</div>
            </div>
            <div style="margin-left: 27%; margin-top: 2%; margin-right: 27%">
              <div
                class="d-flex align-items-center justify-content-center extra-content"
              >
                <p>
                  I’m always excited to connect! Feel free to reach out through
                  the platforms below. Whether you have a question or just want
                  to say hello, I’d love to hear from you.
                </p>
              </div>
              <div
                class="d-flex align-items-center justify-content-center"
                style="margin-top: 3%"
              >
                <img
                  class="line-svg"
                  src="../assets/separatorBlack 1.svg"
                  alt=""
                />
              </div>
              <div
                class="social-icons-big mt-5 d-flex align-items-center justify-content-center"
              >
                <img
                  class="pointer"
                  @click="gitRepo()"
                  src="../assets/git.svg"
                  alt="GitHub"
                />
                <img
                  @click="linkedin()"
                  class="ml-3 pointer"
                  src="../assets/linkedin.svg"
                  alt="LinkedIn"
                />
                <a href="mailto:nayakpavani676@gmail.com">
                  <img
                    class="ml-3 pointer"
                    src="../assets/gmail.svg"
                    alt="gmail"
                  />
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <Footer  @scrollToTop="scrollToTop" />
  </div>
</template>
<script>
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";

export default {
  components: {
    Footer,
    Header,
  },
  data() {
    return {
      readMore: false, // Controls whether to show the "ABOUT ME" box and additional content
      linkedinLink:
        "https://www.linkedin.com/in/pavani-nayak-94b883212?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app", // LinkedIn profile link
      gitLink: "https://github.com/Nayak-Pavani/",
    };
  },
  methods: {
    scrollToSection(sectionId) {
      console.log(sectionId);
      
      const element = document.getElementById(sectionId);
      if (element) {
        element.scrollIntoView({ behavior: "smooth" });
      }
    },
    scrollToTop() {
      console.log("lkjh");

      const element = document.getElementById("main-content");
      if (element) {
        element.scrollIntoView({ top: 1000, behavior: "smooth" });
      }
    },
    gitRepo() {
      window.open(this.gitLink, "_blank"); // Opens the GitHub repository in a new tab
    },
    linkedin() {
      window.open(this.linkedinLink, "_blank"); // Opens the LinkedIn profile in a new tab
    },

    toggleReadMore() {
      this.readMore = !this.readMore; // Toggle readMore state when "READ MORE" is clicked
    },
  },
};
</script>

<style scoped>
.icon-container img{
width: 8vh;
height: 8vh;
}

.icon {
  width: 50px; /* Adjust size as needed */
  height: 50px; /* Adjust size as needed */
  transition: transform 0.3s ease; /* Smooth transition for scaling effect */
}

.icon-container:hover .icon {
  transform: scale(1.2); /* Enlarge the icon on hover */
}

.icon-container {
  animation: popOut 10s infinite; /* Apply the animation */
  animation-delay: 0s; /* Default delay */
}

/* Sequential pop-out animation */
.icon1 {
  animation-delay: 0s;
}
.icon2 {
  animation-delay: 2s;
}
.icon3 {
  animation-delay: 4s;
}
.icon4 {
  animation-delay: 6s;
}
.icon5 {
  animation-delay: 8s;
}
.icon6 {
  animation-delay: 10s;
}
.icon7 {
  animation-delay: 12s;
}
.icon8 {
  animation-delay: 14s;
}
.icon9 {
  animation-delay: 16s;
}
.icon10 {
  animation-delay: 18s;
}
.icon11 {
  animation-delay: 20s;
}

@keyframes popOut {
  0% {
    transform: scale(1);
    opacity: 1;
  }
  50% {
    transform: scale(1.2); /* Enlarge the icon */
    opacity: 1;
  }
  100% {
    transform: scale(1); /* Return to original size */
    opacity: 1;
  }
}

.icon-name {
  display: block; /* Ensure text is on a new line */
  margin-top: 5px; /* Space between image and text */
  font-size: 0.9rem; /* Adjust font size as needed */
  color: #333; /* Adjust text color as needed */
}

/* Container for the entire page */

.line-svg {
  height: auto; /* Maintain aspect ratio */
  margin: 0 30px; /* Equal spacing between the lines and the text */
}
.icon-container {
  text-align: center;
  margin-top: 1rem;
}
.profile-page {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.usingnow-text {
  font-size: 1.5rem;
  font-weight: bold;
  letter-spacing: 8px;
}
.about-me-box {
  border: 5px solid black;
  padding: 12px;
  font-size: 1.5rem;
  font-weight: bold;
  letter-spacing: 8px;
  text-align: center;
  width: 15%;
}
.icon-name {
  display: block;
  font-size: 1rem;
  font-weight: 500;
  color: #333;
  letter-spacing: 3px;
}

/* Layout and spacing for the content (text and image) */
.content {
  margin-left: 21%;
  margin-right: 21%;
  margin-top: 10%;
}

/* Text content section */
.text-content {
  max-width: 50%; /* Take 50% of the container width */
}

.hai-text {
  font-size: 1.8rem;
  color: black;
  font-weight: 600;
}

.name-text {
  font-size: 2.4rem;
  color: black;
  font-weight: 700;
}

.developer-text {
  font-size: 1.6rem;
  color: #555;
}
.line-svg-right {
  margin-left: 2vh;
}

.social-icons img {
  width: 30px;
  height: 30px;
}
.social-icons-big img {
  width: 60px;
  height: 60px;
}

.social-icons img.ml-3 {
  margin-left: 15px;
}
.social-icons-big img.ml-3 {
  margin-left: 15px;
}

/* Profile image section */
.profile-image img {
  width: 200px; /* Adjust the width */
  border-radius: 50%;
}

/* About Me section */
.about-me {
  background-color: black;
  color: white;
  padding: 20px;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  box-sizing: border-box; /* Make sure padding is included in width */
}

.about-me-text {
  font-size: 1rem;
  margin-left: 10%;
  padding: 20px;
  line-height: 1.6;
}
.extra-content p {
  font-weight: 500;
  font-size: 1rem;
  line-height: 1.6;
  color: black;
  margin: 0; /* Remove default margin */
  padding: 0; /* Remove default padding */
  text-align: center; /* Center-align the text */
}
.explore-text {
  font-weight: 600;
  font-size: 1.5rem;
  line-height: 1.6;
  color: black;
}
.readmore-text {
  position: relative;
  color: white;
  font-weight: bold;
  cursor: pointer;
}
html {
  scroll-behavior: smooth;
}
.pointer {
  cursor: pointer;
}
.readmore-text::after {
  content: " ";
  position: absolute;

  top: 50%;
  transform: translateY(-50%);
  width: 24px;
  height: 24px;
  background: url("../assets/git.svg") no-repeat center center;
  background-size: contain;
  animation: bounce 1s infinite;
}

@keyframes bounce {
  0%,
  100% {
    transform: translateY(-50%) translateX(0);
  }
  50% {
    transform: translateY(-50%) translateX(10px);
  }
}
/* Responsive Design for smaller screens */
@media (max-width: 768px) {
  .d-flex {
    flex-direction: column;
    align-items: center;
  }

  .text-content {
    max-width: 100%;
    text-align: center;
  }

  .profile-image {
    margin-top: 20px;
  }

  .about-me-text {
    margin-left: 5%; /* Reduce margin for smaller screens */
  }
}
</style>
