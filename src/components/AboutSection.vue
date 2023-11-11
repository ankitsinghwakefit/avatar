<template>
   <div>
    <div class="hero-container">
      <div md class="intro">
        <h1>About me</h1><br />
        <h4>Hey, I'm Tania! I'm a software developer working in Chicago. Welcome to my spot on the web for my projects, tutorials, art, musings, and anything else I want to show the world. Check out the projects page to see a highlight of my open-source work, and the blog for my tutorials and more.</h4><br />
        <h4>My site has no ads, no affiliate links, no tracking or analytics, no sponsored posts, and no paywall. My only motivation for this site is to share what I've learned with the world. Although the tide is against me, I want to make the internet a better place, even if it's just right here. I hope I will inspire others to make their own creative corner on the web as well.</h4><br />
        <!-- <h4>You can contact me by email at <u><strong>hello</strong></u> at <u><strong>taniarascia.com</strong></u> to say hi! I always appreciate meeting new people.</h4><br />
        <ul>
          <li><a href="https://taniarascia.substack.com">Newsletter</a></li>
          <li><a href="https://github.com/taniarascia">GitHub</a></li>
          <li><a href="https://twitter.com/taniarascia">Twitter</a></li>
        </ul> -->
      </div>
      <div md class="image">
      <div class="post-sidebar-card">
        <h2>Me</h2>
        <img src="@/assets/ankit.jpg" alt="Tania">
      </div>
        <!-- <img src="@/assets/ram.png" alt="ram"> -->
      </div>
    </div>
    <div class="details-container">
      <h4>You can contact me by email at <u><strong>hello</strong></u> at <u><strong>taniarascia.com</strong></u> to say hi! I always appreciate meeting new people.</h4><br />
      <ul>
        <li><a href="https://taniarascia.substack.com">Newsletter</a></li>
        <li><a href="https://github.com/taniarascia">GitHub</a></li>
        <li><a href="https://twitter.com/taniarascia">Twitter</a></li>
      </ul>
      <h2>Tools</h2>
      <h3>Software</h3>
      <ul>
        <li>This website is hosted on <a href="https://netlify.com">Netlify</a> and uses the <a href="https://www.gatsbyjs.com/">Gatsby</a> framework</li>
        <li><strong>Coding</strong>: <a href="https://code.visualstudio.com/">Visual Studio Code</a> with <a href="https://taniarascia.github.io/new-moon">New Moon Theme</a></li>
        <li><strong>Terminal</strong>: <a href="https://iterm2.com/">iTerm2</a></li>
        <li><strong>Notes</strong>: <a href="https://obsidian.md/">Obsidian</a></li>
        <li><strong>Music</strong>: <a href="https://www.spotify.com/">Spotify</a></li>
      </ul>
      <h3>Hardware</h3>
      <ul>
        <li><strong>Coding PC</strong>: M1 MacBook Pro 16" 2021</li>
        <li><strong>Gaming PC</strong>
        <ul>
        <li>CPU: <a href="https://www.amd.com/en/products/cpu/amd-ryzen-5-3600">AMD Ryzen 5 3600</a></li>
        <li>Motherboard: <a href="https://www.asrock.com/MB/AMD/B550%20Phantom%20Gaming%204/index.asp">ASRock B550 Phantom Gaming 4</a></li>
        <li>Memory: <a href="https://www.crucial.com/memory/ddr4/bl2k16g36c16u4b">Crucial Ballistix 32GB</a></li>
        <li>Storage: <a href="https://www.samsung.com/us/computing/memory-storage/solid-state-drives/ssd-970-evo-nvme-m-2-1tb-mz-v7e1t0bw/">SSD 970 EVO NVMe M.2 1TB</a></li>
        <li>GPU: <a href="https://www.nvidia.com/en-us/geforce/graphics-cards/gtx-1660-ti/">GTX 1660Ti</a></li>
        <li>PSU: <a href="https://www.evga.com/products/product.aspx?pn=120-GP-0650-X1">EVGA SuperNOVA 650 G+</a></li>
        <li>Case: <a href="https://nzxt.com/product/h510-elite">H510 Elite</a></li>
        </ul>
        </li>
        <li><strong>Monitor</strong>: <a href="https://www.asus.com/us/displays-desktops/monitors/tuf-gaming/tuf-gaming-vg27aq/">TUF Gaming VG27AQ (x2)</a></li>
        <li><strong>Keyboard</strong>: <a href="https://www.durgodkeyboard.com/product/durgod-fusion-65-bluetooth-5-0-2-4g-wireless-mechanical-keyboard-cherry-switch-type-c-software-macro-nkro-pbt-doubleshot-keycap/">Durgod Fusion</a></li>
        <li><strong>Microphone</strong>: <a href="https://www.bluemic.com/en-us/products/yeti/">Blue Yeti</a></li>
        <li><strong>Headphones</strong>: <a href="https://www.sony.com/electronics/headband-headphones/wh-1000xm3">Sony WH-1000XM3</a></li>
      </ul>
      <h2>Books</h2>
      <ul>
        <li><a href="https://www.digitalocean.com/community/books/understanding-the-dom-document-object-model-ebook">Understanding the DOM</a>
        </li>
        <li>Secrets of javascript</li>
        <li>Eloquent javascript</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
 .hero-container {
  display: flex;
  align-items: center;
}
.intro {
  width: 60%;
  padding: 90px 10px;
  color: #f9f9f9 !important;
}
.post-sidebar-card {
    background: #1f1f1f;
    border: 1px solid #2c2c2c;
    border-radius: 6px;
    margin: 1rem 0;
    padding: 1.5rem;
}
.post-sidebar-card h2 {
    border: none;
    color: white;
    font-size: .9rem;
    font-weight: 700;
    letter-spacing: 0;
    margin: 0 0 1rem;
    text-transform: uppercase;
}
h1 {
  font-size: 4rem !important;
    font-family: Inter,-apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
  font-weight: 700;
}
h2 {
  border-bottom: 1px solid #2c2c2c;
  color: white;
  font-family: Inter,-apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
  font-size: 1.8rem;
  font-weight: 700;
  letter-spacing: -.05rem;
  margin: 0 0 1rem;
  padding-bottom: 0.4rem;
}
h3 {
  color: white;
  font-family: Inter,-apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
  font-size: 1.5rem;
  font-weight: 500;
  margin-bottom: 1.25rem;
}
h4 {
  font-size: 1.2rem;
  font-weight: 400;
  font-family: Inter,-apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
  word-spacing: 1px;
  color: #e6e6e6;
}
.image {
  width: 25%;
  margin-left: 70px;
}
img {
  width: -webkit-fill-available;
}
ul li a {
  color: #9ca0fa;
  text-decoration: none;
  font-size: 19px;
}
ul {
  color: #e6e6e6;
   font-size: 19px;
}
ul li::before {
  content: "\2022";
  color: pink;
  font-weight: bold;
  display: inline-block; 
  width: 1em;
  margin-left: -1em;
  font-size: 30px;
}
.details-container {
  padding: 0px 10px;
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