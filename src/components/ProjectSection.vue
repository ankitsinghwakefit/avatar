<template>
<div>
  <div class="project-container">
    <div class="projects">Latest Projects</div>
    <div class="button"><button>View All</button></div>
  </div>
    <!-- <div class="project-section">
      <div class="project-box" v-for="project in projects" :key="project.id">
        <div class="project-name">{{project.name}}</div>
        <div class="project-date">{{project.createdOn}}</div>
      </div>
    </div> -->
    <!-- <b-card-group class="project-card-section">
      <b-card class="card-wrapper" v-for="project in projects" :key="project.id">
        <card-Component :title="project.title" :year="project.year" :description="project.description" :demo-link="project.demoLink" />
      </b-card>
    </b-card-group> -->
    <!-- <div class="main-section"> -->
  <!-- <div class="card" v-for="project in projects" :key="project.id">
    <div>
      <time>{{project.year}}</time>
      <a class="card-header" :href="project.demoLink" target="_blank">{{project.title}}</a>
      <p>{{project.description}}</p>
    </div>
    <div class="anchored links">
      <a class="button" target="_blank" :href="project.articleLink">Article</a>
      <a class="button flex" target="_blank" :href="project.demoLink">Demo</a>
    </div>
  </div> -->
  <!-- <div class="card"></div>
  <div class="card"></div>
  <div class="card"></div>
  <div class="card"></div>
  <div class="card"></div>
  <div class="card"></div> -->
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
            <a class="button small" href="/musical-instrument-web-audio-api"
              >Article</a
            ><a
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
              :href="project.articleLink"
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
<!-- </div>  -->
    </div>
</template>

<script>
// import CardComponent from "@/components/molecules/cardComponent.vue";
export default {
  data(){
    return  {
      projects: [
        {id: "1", title: "Car Racing", year: "2020", description: "Prototype of car race", demoLink: "https://neon-platypus-a5c384.netlify.app/", articleLink: "#"},
        {id: "2", title: "Standalone Dropdown", year: "2021", description: "Prototype of dropdown", demoLink: "https://peaceful-lamarr-7f3e3d.netlify.app/", articleLink: "#"},
        {id: "3", title: "John Wiley & Sons", year: "2022", description: "Learning anything easy", demoLink: "https://www.dummies.com/", articleLink: "https://www.dummies.com/about-for-dummies/"},
        {id: "4", title: "Telefónica Germany", year: "2023", description: "WhatsApp SIM", demoLink: "https://www.whatsappsim.de/plp.html", articleLink: "https://www.telefonica.de/news/corporate/2020/02/whatsapper-aufgepasst-whatsapp-sim-stockt-tarifoptionen-deutlich-auf-und-ueberarbeitet-app-design.html"},
      ],
    }
  },
  // components: {
  //   CardComponent,
  // }
}
</script>


<style scoped>
.project-container {
  color: #f9f9f9;
  align-items: center;
  border: 0;
  display: flex;
  justify-content: space-between;
  margin-bottom: 2rem;
  margin-top: 2rem;
  padding: 0;
}
.projects {
  font-size: 3rem;
  font-weight: 700;
}
button {
  align-items: center;
  background: rgb(37, 37, 37);
  border: 1px solid rgb(44, 44, 44);
  border-radius: 6px;
  color: rgb(230, 230, 230);
  cursor: pointer;
  display: inline-flex;
  font-size: 1rem;
  font-weight: 500;
  gap: 0.25rem;
  letter-spacing: 0;
  line-height: 1;
  padding: 0.75rem 1.2rem;
  white-space: nowrap;
}
.project-box {
  display: flex;
  font-size: 1.5rem;
  font-weight: 600;
  background: transparent;
  border-bottom: 1px solid #2c2c2c;
  gap: 1rem;
  padding: 0.4rem 0;
  text-decoration: none;
  justify-content: space-between;
}
.project-name {
  color: white;
}
.project-date {
  color: #5eddac;
}
.project-card-section {
  font-size: 1.5rem;
  padding: 0.4rem 0;
  text-decoration: none;
  gap: 2rem;
}
.card-body {
  padding: 0px !important;
}
.main-section {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  background: #181818;
}
/*
.card {
  min-width: 400px;
  margin: 16px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background: #fff;
  box-sizing: border-box;
    background: #1f1f1f;
      border: 1px solid #2c2c2c;
      border-radius: 6px;
      padding: 2rem;
}
.card time {
  color: #f57ad0;
    display: block;
    font-family: Menlo,"IBM Plex Mono",Menlo,monospace;
    font-size: 1.3rem;
    letter-spacing: -.01rem;
}
.card a.card-header {
  border: 0;
  color: white;
  display: block;
  font-family: "Inter",-apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
  font-size: 1.5rem;
  font-weight: 500;
  line-height: 1.3;
  margin: 0.1rem 0 0.5rem;
  padding: 0;
  text-decoration: none;
}
.card p {
    color: #999;
    font-family: "Inter",-apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
    font-size: 1rem;
    line-height: 1.5;
    margin: 0;
    margin-bottom: 20px;
}
.links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}
a.button {
    align-items: center;
    -webkit-appearance: none;
    background: #252525;
    border: 1px solid #2c2c2c;
    border-radius: 6px;
    color: #e6e6e6;
    cursor: pointer;
    display: inline-flex;
    font-family: -apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
    font-size: 1rem;
    font-weight: 500;
    gap: 0.25rem;
    letter-spacing: 0;
    line-height: 1;
    padding: 0.75rem 1.2rem;
    white-space: nowrap;
    text-decoration: none;
}
a.button:hover {
  border: 1px solid #3d3d3d;
}
*/
@media screen and (max-width: 912px){
  /*
  .projects {
  font-size: 2rem;
  font-weight: 700;
}
.card {
  min-width: 340px;
}
*/
}
@media screen and (max-width: 790px){
  /*
  .card {
  width: 100%;
  margin: 16px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background: #fff;
  box-sizing: border-box;
   background: #1f1f1f;
      border: 1px solid #2c2c2c;
      border-radius: 6px;
      padding: 2rem;
}
*/
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