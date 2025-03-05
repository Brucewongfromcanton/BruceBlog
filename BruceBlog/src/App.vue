<script setup>
</script>

<template>
  <header>
    <a href="\App.vue">
      <img src=\android-chrome-192x192.png alt="Favicon" style="width: 64px; height: 64px;">
    </a>
    <a href="\App.vue">
      <h1>BruceBlog</h1>
    </a>
  </header>
  <div>
    <li><span>About me</span></li>
    <li><span>Projects</span></li>
    <li><span>Gallery</span></li>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
@import url('https://fonts.cdnfonts.com/css/minecraft-4');
  

  header {
    display: flex;
    align-items: center;
    font-family: 'Minecraft', sans-serif;
  }
  
  a {
    text-decoration: none;
    color: black;
  }

  div {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 90vh;
    text-align: left;
  }

  li {
    padding: 15px;
    font-family: "Montserrat", serif;
    font-size: 30px;
    list-style-type: none;
    width: 30%;
    cursor: pointer; /* Add cursor pointer for better UX */
    position: relative; /* Required for the pseudo-element */
  }

  li span {
    position: relative; /* Required for the pseudo-element */
  }

  li span::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: -2px; /* Position the underline just below the text */
    width: 0;
    height: 2px;
    background-color: black;
    transition: width 0.3s ease-in-out; /* Animation effect */
  }

  li span:hover::after {
    width: 100%; /* Expand the underline on hover */
  }
</style>

