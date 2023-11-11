<template>
  <div>
    <div class="hero-container">
      <div md class="intro">
      <h1>Hey, I'm Ankit!</h1><br />
      <h4>Welcome to my digital garden. 🌱</h4><br />
      <h4>I'm a software developer in India. I make <a href="#">open-source projects</a> and <a href="#">write</a> about code, design, and life. I like accordions, drawing, sci-fi, reading, and gaming.</h4>
      </div>
      <div md class="image"><img src="@/assets/ram.png" alt="ram"></div>
    </div>
  </div>
</template>

<style scoped>
.hero-container {
  display: flex;
      align-items: center;
}
.intro {
  width: 50%;
  padding: 90px 10px;
  color: #f9f9f9 !important;
}
h1 {
  font-size: 4rem !important;
}
h3 {
  line-height: 1.6;
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