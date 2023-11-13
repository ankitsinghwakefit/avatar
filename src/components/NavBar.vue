<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
      <b-navbar-brand active :to="{name: 'about'}">About</b-navbar-brand>
      <b-navbar-brand :to="{name: 'projects'}">Projects</b-navbar-brand>
      <b-navbar-brand :to="{name: 'journey'}">Journey</b-navbar-brand>
      <b-navbar-brand href="https://github.com/ankitsinghwakefit" target="_blank">Github</b-navbar-brand>
      <b-navbar-brand :to="{name: 'home'}">Home</b-navbar-brand>
      <!-- <b-navbar-toggle target="nav-collapse"></b-navbar-toggle> -->

      <!-- <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Projects</b-nav-item>
          <b-nav-item href="#">Journey</b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav class="ml-auto">
          <b-navbar-nav>
            <b-nav-item href="#">Github</b-nav-item>
          </b-navbar-nav>
        </b-navbar-nav>
      </b-collapse> -->
    </b-navbar>
  </div>
</template>

<style scoped>
.bg-info {
  background-color: #181818 !important;
}
.navbar-brand {
  color: #bbbbbb !important;
  font-size: 18px !important;
}
.navbar-brand:hover {
  border-bottom: 3px solid #bbb;
}
.nav-link {
font-size: 20px !important;
}
@media screen and (max-width: 900px){
  .bg-info {
  border-bottom: .5px solid rgb(44, 44, 44) !important;
}
}
</style>