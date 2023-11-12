<template>
  <footer class="footer">
    <section>
    <nav>
      <span>Made by Ankit Singh</span>
      <a href="https://github.com/ankitsinghwakefit" title="GitHub" target="_blank" rel="noopener noreferrer"><span>GitHub</span><img src="@/assets/git.png" alt="GitHub"></a>
      <a href="https://www.netlify.com" title="Netlify" target="_blank" rel="noopener noreferrer"><span>Netlify</span><img src="@/assets/netlify.png" alt="Netlify"></a>
      <a href="https://vuejs.org/" title="vuejs" target="_blank" rel="noopener noreferrer"><span>Vue</span><img src="@/assets/logo.png" alt="vue"></a>
    </nav>
    </section>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
.footer {
   font-family: Inter,-apple-system,BlinkMacSystemFont,"Helvetica Neue",Arial,sans-serif;
    padding: 3rem 0;
}
.footer section {
    align-items: center;
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
}
.footer nav {
    display: flex;
    gap: 0.25rem;
    margin: 0 1rem;
}
.footer a, .footer span {
    align-items: center;
    color: #e6e6e6;
    display: flex;
    font-size: 1rem;
    line-height: 1.2;
    padding: 0 0.5rem;
    text-decoration: none;
}
.footer img {
    display: inline-block;
    max-height: 20px;
    width: auto;
}
.footer span {
    align-items: center;
    color: #e6e6e6;
    display: flex;
    font-size: 1rem;
    line-height: 1.2;
    padding: 0 0.5rem;
}
</style>