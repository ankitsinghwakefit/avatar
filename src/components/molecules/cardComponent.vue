<template>
  <div class="card">
    <p>{{year}}</p>
    <p>{{title}}</p>
    <p>{{description}}</p>
    <p>{{demoLink}}</p>
  </div>
</template>

<script>

export default({
  props: {
    year: {
      type: String,
      default: "2020",
    },
    title: {
      type: String,
      default: "title",
    },
    description: {
      type: String,
      default: "description",
    },
    demoLink: {
      type: String,
      default: "#"
    }
  }
})
</script>


<style scoped>
.card {
    background: #1f1f1f;
    border: 1px solid #2c2c2c;
    border-radius: 6px;
    padding: 1.5rem;
}
.card-body {
  padding: 0px !important;
}
</style>