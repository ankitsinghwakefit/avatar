<template>
  <div class="home-wrapper">
    <b-container fluid>
      <h1><img class="logo" src="@/assets/floppylogo.png" /> Ankit Singh</h1>
      <b-row>
        <b-col><nav-bar /></b-col>
      </b-row>
      <h1 class="project-heading">Projects</h1>
      <div class="project-preview">
        <div
          v-for="project in projects"
          :key="project.id"
          class="card anchored large"
        >
          <div>
            <time>{{project.year}}</time>
            <a
              class="card-header"
              href="#"
              target="_blank"
              rel="noreferrer"
              >{{project.title}}</a
            >
            <p>{{project.description}}</p>
          </div>
          <div class="links anchored">
            <a
              class="button small flex"
              :href="project.demoLink"
              target="_blank"
              rel="noreferrer"
              >Demo
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                style="width: 1rem; height: 1rem; fill: currentColor"
              >
                <g data-name="Layer 2">
                  <g data-name="external-link">
                    <rect width="24" height="24" opacity="0"></rect>
                    <path
                      d="M20 11a1 1 0 0 0-1 1v6a1 1 0 0 1-1 1H6a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h6a1 1 0 0 0 0-2H6a3 3 0 0 0-3 3v12a3 3 0 0 0 3 3h12a3 3 0 0 0 3-3v-6a1 1 0 0 0-1-1z"
                    ></path>
                    <path
                      d="M16 5h1.58l-6.29 6.28a1 1 0 0 0 0 1.42 1 1 0 0 0 1.42 0L19 6.42V8a1 1 0 0 0 1 1 1 1 0 0 0 1-1V4a1 1 0 0 0-1-1h-4a1 1 0 0 0 0 2z"
                    ></path>
                  </g>
                </g></svg></a
            ><a
              class="button small flex"
              :href="project.sourceLink"
              target="_blank"
              rel="noreferrer"
              >Source
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                style="width: 1rem; height: 1rem; fill: currentColor"
              >
                <g data-name="Layer 2">
                  <g data-name="external-link">
                    <rect width="24" height="24" opacity="0"></rect>
                    <path
                      d="M20 11a1 1 0 0 0-1 1v6a1 1 0 0 1-1 1H6a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h6a1 1 0 0 0 0-2H6a3 3 0 0 0-3 3v12a3 3 0 0 0 3 3h12a3 3 0 0 0 3-3v-6a1 1 0 0 0-1-1z"
                    ></path>
                    <path
                      d="M16 5h1.58l-6.29 6.28a1 1 0 0 0 0 1.42 1 1 0 0 0 1.42 0L19 6.42V8a1 1 0 0 0 1 1 1 1 0 0 0 1-1V4a1 1 0 0 0-1-1h-4a1 1 0 0 0 0 2z"
                    ></path>
                  </g>
                </g></svg
            ></a>
          </div>
        </div>
      </div>
    </b-container>
    <footer-section />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from "@/components/NavBar.vue";
import FooterSection from "@/components/FooterSection.vue";
import projectsData from "@/assets/projectData/projects.json";
export default {
  name: "ProjectView",
  components: {
    NavBar,
    // JourneySection,
    FooterSection,
  },
  data() {
    return {
      projects: projectsData,
    };
  },
};
</script>

<style scoped>
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
.project-heading {
  color: #f9f9f9 !important;
  font-size: 30px !important;
  margin: 2rem 0rem !important;
}
.project-preview {
  display: grid;
  gap: 1rem;
}
.card {
  background: #1f1f1f !important;
  border: 1px solid #2c2c2c !important;
  border-radius: 6px;
  padding: 1rem;
  position: relative;
}
.stars {
  position: absolute;
  right: 1rem;
  top: 1rem;
}
.project-preview .card time {
  color: #f6cd5d;
}
.card time {
  color: var(--card-time-color);
  display: block;
  font-family: Menlo, "IBM Plex Mono", Menlo, monospace;
  font-size: 0.9rem;
  letter-spacing: -0.01rem;
}
.card a.card-header,
.card h2 {
  border: 0;
  color: white;
  display: block;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Helvetica Neue",
    Arial, sans-serif;
  font-size: 1rem;
  font-weight: 500;
  line-height: 1.3;
  margin: 0.1rem 0 0.5rem;
  padding: 0;
  text-decoration: none;
}
.card p {
  color: #999;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "Helvetica Neue",
    Arial, sans-serif;
  font-size: 0.9rem;
  line-height: 1.5;
  margin: 0;
}
.links, .tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}
a.button.small, button.small {
    font-size: .9rem;
    padding: 0.5rem 0.6rem;
}
a.button, button {
    align-items: center;
    -webkit-appearance: none;
    background: #252525;
    border: 1px solid #2c2c2c;
    border-radius: 6px;
    color: #e6e6e6;
    cursor: pointer;
    display: inline-flex;
    font-size: 1rem;
    text-decoration: none;
    font-weight: 500;
    gap: 0.25rem;
    letter-spacing: 0;
    line-height: 1;
    padding: 0.75rem 1.2rem;
    white-space: nowrap;
}
a.button:hover, button:hover {
    border-color: #666;
    color:white;
}
@media screen and (min-width: 1060px) {
  .project-preview {
    grid-template-columns: repeat(3, 1fr);
  }
}
@media screen and (min-width: 700px) {
  .project-preview {
    grid-template-columns: repeat(2, 1fr);
  }
  .stars {
    right: 1.5rem;
    top: 1.5rem;
  }
  .card.anchored {
    padding-bottom: 3.5rem;
  }
  .card.anchored.large {
    padding-bottom: 5rem;
  }
  .card {
    padding: 1.5rem;
  }
  .card a.card-header,
  .card h2 {
    font-size: 1.1rem;
    font-weight: 500;
  }
  .links.anchored {
    bottom: 1.5rem;
    left: 1.5rem;
    position: absolute;
}
.links {
    margin-top: 1rem;
}
}
@media screen and (max-width: 900px) {
  .home-wrapper {
    background-color: rgb(24, 24, 24);
    padding: 20px 0px;
  }
}
</style>
