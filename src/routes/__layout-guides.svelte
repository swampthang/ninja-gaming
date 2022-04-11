<script>
    import Title from '$lib/title.svelte';
    import '../styles/global.css';
</script>

<header>
  <nav>
    <Title title="Ninja Gaming Guides" />
    <div class="links">
      <a href="/">Home</a>
      <a href="/about">About</a>
      <a href="/guides">Guides</a>
    </div>
  </nav>
</header>

<main>
    <!-- page content -->
    <slot></slot>
</main>

<footer>
  <p>Copyright 2022 Ninja Gaming Guides</p>
</footer>

<style>
  main {
    max-width: 960px;
    margin: 20px auto;
  }
  header {
    text-align: center;
    background: rgba(0,0,0,0.1);
  }
  .links {
    margin-left: auto;
  }
  a {
    margin-left: 10px;
  }
  nav {
    display: flex;
    align-items: center;
    max-width: 960px;
    margin: 0 auto;
  }
  footer {
    text-align: center;
  }
</style>