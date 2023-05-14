<template>
    <div class="video-background">
      <video autoplay muted loop>
        <source src="~/assets/pexels-rostislav-uzunov-10613972-1920x1080-24fps.mp4" type="video/mp4">
      </video>
      <div class="overlay">
        <nav class="navbar">
          <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact Us</a></li>
            <li><a href="#login">Login</a></li>
            <li><a href="#register">Register</a></li>
          </ul>
        </nav>
        <div class="content">
            <!-- <flamingtext></flamingtext> -->
            <h1>THE POWER OF FRIENDSHIP</h1>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
          <button class="join-button" @click="redirectToVideo">Join Now</button>
        </div>
      </div>
    </div>
  </template>

<script>
export default {
  methods: {
    redirectToVideo() {
      window.location.href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ&t=11s&ab_channel=RickAstley";
    }
  }
};
</script>
  
  
  <style scoped>
  .video-background {
    position: relative;
    width: 100%;
    height: 100vh;
    overflow: hidden;
  }
  
  .video-background video {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    min-width: 100%;
    min-height: 100%;
    width: auto;
    height: auto;
    z-index: -1;
    filter: blur(10px);
  }
  
  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    z-index: 1;
  }
  
  .navbar {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.7); /* Black background color with opacity */
    padding: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 2;
  }
  
  .nav-links {
    list-style: none;
    display: flex;
  }
  
  .nav-links li {
    margin: 0 1rem;
  }
  
  .nav-links a {
    color: white;
    text-decoration: none;
    font-size: 1.2rem;
    transition: color 0.3s;
  }
  
  .nav-links a:hover {
    color: #ffcd00;
  }
  
  .content {
    text-align: center;
    color: white;
    margin-top: 5rem; /* Add some margin to avoid content overlapping with the fixed navbar */
  }
  
  h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
  }
  
  p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
  }
  
  .join-button {
    background-color: #ffffff;
    color: #000000;
    padding: 1rem 2rem;
    font-size: 1.5rem;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  </style>
  