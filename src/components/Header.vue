<template>
    <div class="header">
      <b-container class="bv-example-row">
        <b-row class="align-items-center">
          <!-- First column: Pavani's Portfolio (aligned to the left) -->
          <b-col cols="auto" class="portfolio-col">
            <span class="portfolio-text">Pavani's Portfolio</span>
          </b-col>
  
          <!-- Remaining columns should be aligned to the right -->
          <b-col class="nav-wrapper">
            <b-nav class="custom-nav">
              <b-nav-text class="nav-item pointer">About Me</b-nav-text>
              <b-nav-text class="nav-item pointer">Projects</b-nav-text>
              <b-nav-text class="nav-item pointer">Skills</b-nav-text>
              <b-nav-text class="nav-item pointer">Contact Me</b-nav-text>
              <b-button  pill variant="primary" class="custom-button pointer">Resume</b-button>
            </b-nav>
          </b-col>
        </b-row>
      </b-container>
     
    </div>
  </template>
  
  <script>
  export default {};
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
    font-size: 2rem; /* Larger font size for Pavani's Portfolio */
    color: black;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Drop shadow */
    font-weight: 600;
  }
  
  .nav-wrapper {
    display: flex;
    justify-content: space-around; /* Align items to the right */
    flex: 1; /* Take up remaining space */
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
    color: rgb(255, 255, 255) !important; /* Force black color for all nav items */
    text-shadow: 1px 1px 3px rgba(102, 102, 102, 0.3); /* Drop shadow */
    text-decoration: none; /* Remove default underline */
    position: relative; /* For positioning the underline */
    padding: 0 15px; /* Add horizontal padding for spacing */
    transition: color 0.3s ease; /* Smooth color transition */
  }
  
  .nav-item:hover {
    color: rgb(255, 255, 255) !important; /* Ensure text color remains black on hover */
  }
  
  .nav-item::after {
    content: ''; /* Pseudo-element for the underline */
    display: block;
    position: absolute;
    left: 0;
    bottom: 0; /* Position the underline just below the text */
    width: 0;
    height: 2px;
    background: rgb(255, 255, 255); /* Underline color */
    transition: width 0.3s ease; /* Smooth transition */
  }
  
  .nav-item:hover::after {
    width: 100%; /* Full width underline on hover */
  }
  
  .custom-button {
    margin-left: 20px;
  border: 2px solid rgb(255, 255, 255) !important; /* Black border */
  color: rgb(255, 255, 255) !important; /* Black text color */
  background-color: transparent !important; /* Transparent background */
  transition: background-color 0.3s ease, color 0.3s ease; /* Smooth transition */
}

.custom-button:hover {
  background-color: rgb(255, 255, 255) !important; /* Black background on hover */
  color: rgb(0, 0, 0) !important; /* White text color on hover */
  border-color: rgb(255, 255, 255) !important; /* Ensure border color stays black */
}
  .pointer{
    cursor: pointer; /* Change cursor to pointer for clickable elements */
  }
  </style>
  