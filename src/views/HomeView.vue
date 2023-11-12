<template>
  <div class="home-wrapper">
    <b-container fluid>
    <h1><img class="logo" src="@/assets/floppylogo.png"/>Ankit Singh</h1>
      <b-row>
        <b-col><nav-bar /></b-col>
      </b-row>
      <hero-section />
      <project-section />
    </b-container>
    <footer-section />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from "@/components/NavBar.vue";
import HeroSection from "@/components/HeroSection.vue";
import FooterSection from "@/components/FooterSection.vue";
import ProjectSection from "@/components/ProjectSection.vue";
export default {
  name: "HomeView",
  components: {
    NavBar,
    HeroSection,
    ProjectSection,
    FooterSection
  },
};
</script>

<style>
body {
  background-color: #181818;
  color: #fff;
}
.home-wrapper {
  background-color: rgb(24, 24, 24);
  padding: 30px 60px;
}
.logo {
  height: 30px;
  margin-right: 0.25rem;
  max-height: 30px;
  max-width: 30px;
  width: 30px;
}
h1 {
  color: #f9f9f9 !important;
  font-size: 30px !important;
}
@media screen and (max-width: 900px){
  .home-wrapper {
  background-color: rgb(24, 24, 24);
  padding: 20px 0px;
}
}
</style>
