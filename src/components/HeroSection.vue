<template>
  <div>
    <div class="hero-container">
      <div md class="intro">
        <h1>Hey, I'm Ankit!</h1><br />
        <h4>Welcome to my digital garden. 🌱</h4><br />
        <h4>I'm a software developer in India. I make <a href="#">open-source projects</a> and <a href="#">write</a> about code, design, and life. I like accordions, drawing, sci-fi, reading, and gaming.</h4>
      </div>
      <div md class="image">
        <img src="@/assets/ram.png" alt="ram">
      </div>
    </div>
  </div>
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');

.hero-container {
  display: flex;
  align-items: center;
}
.intro {
  width: 50%;
  padding: 90px 10px;
  color: #f9f9f9 !important;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Helvetica Neue",
    Arial, sans-serif;
}
h1 {
  font-size: 3rem !important;
}
h3 {
  line-height: 1.6;
}
h4 {
  font-size: 20px !important;
}
.image {
  width: 40%;
  margin-left: 70px;
}
img {
  width: -webkit-fill-available;
}
@media screen and (max-width: 900px){
   .hero-container {
    display: flex;
    flex-direction: column;
  }
  .intro {
  width: 100%;
  padding: 10px 0px;
  color: #f9f9f9 !important;
}
h1 {
  font-size: 3rem !important;
}
.image {
  width: 100%;
  margin-left: 0px;
}
}
</style>