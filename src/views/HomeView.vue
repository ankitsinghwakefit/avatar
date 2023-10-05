<template>
  <div class="home-wrapper">
    <b-container fluid>
      <b-row>
        <b-col><nav-bar /></b-col>
        <!-- <b-col>2 of 3</b-col>
    <b-col>3 of 3</b-col> -->
      </b-row>
    </b-container>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from "@/components/NavBar.vue";
export default {
  name: "HomeView",
  components: {
    NavBar,
  },
};
</script>

<style>
.home-wrapper {
  background-color: rgb(24, 24, 24);
}
</style>
