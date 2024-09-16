<template>
    <div class="header">
      <b-container class="bv-example-row">
        <b-row class="align-items-center">
          <b-col cols="auto" class="portfolio-col">
            <span class="portfolio-text">Pavani's Portfolio</span>
          </b-col>
  
          <b-col class="nav-wrapper">
            <b-nav class="custom-nav">
            <b-nav-text class="nav-item pointer" @click="scrollTo('about-me')">About Me</b-nav-text>
            <b-nav-text class="nav-item pointer" @click="scrollTo('projects')">Projects</b-nav-text>
            <b-nav-text class="nav-item pointer" @click="scrollTo('skills')">Skills</b-nav-text>
            <b-nav-text class="nav-item pointer" @click="scrollTo('contact-me')">Contact Me</b-nav-text>
            <b-button pill variant="primary" class="custom-button pointer">Resume</b-button>
          </b-nav>
          </b-col>
        </b-row>
      </b-container>
     
    </div>
  </template>
  
  <script>
  export default {
  methods:{
    scrollTo(sectionId) {
      this.$emit('scroll-to-section', sectionId);
    }
  }
  };
  </script>
  
  <style scoped>
 
  .header {
    /* padding: 20px; */
    padding-top: 20px;
    margin-left: 20%;
    margin-right: 20%;
  }
  

  
  .portfolio-col {
    display: flex;
    align-items: center;
  }
  
  .portfolio-text {
    font-style: Montserrat;
    font-size: 2rem; 
    color: black;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); 
    font-weight: 600;
  }
  
  .nav-wrapper {
    display: flex;
    justify-content: space-around; 
    flex: 1; 
  }
  
  .custom-nav {
    display: flex;
    align-items: center;
    padding-left: 0;
    margin-bottom: 0;
    list-style: none;
    margin-left:23%
  }
  
  .nav-item {
    color: rgb(255, 255, 255) !important;
    text-shadow: 1px 1px 3px rgba(102, 102, 102, 0.3); 
    text-decoration: none; 
    position: relative; 
    padding: 0 15px; 
    transition: color 0.3s ease;
  }
  
  .nav-item:hover {
    color: rgb(255, 255, 255) !important; 
  }
  
  .nav-item::after {
    content: ''; 
    display: block;
    position: absolute;
    left: 0;
    bottom: 0; 
    width: 0;
    height: 2px;
    background: rgb(255, 255, 255); 
    transition: width 0.3s ease; 
  }
  
  .nav-item:hover::after {
    width: 100%;
  }
  
  .custom-button {
    margin-left: 20px;
  border: 2px solid rgb(255, 255, 255) !important; 
  color: rgb(255, 255, 255) !important; 
  background-color: transparent !important; 
  transition: background-color 0.3s ease, color 0.3s ease; 
}

.custom-button:hover {
  background-color: rgb(255, 255, 255) !important;
  color: rgb(0, 0, 0) !important; 
  border-color: rgb(255, 255, 255) !important; 
}
  .pointer{
    cursor: pointer; 
  }
  </style>
  