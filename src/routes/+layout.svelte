<nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/posts">Posts</a>
</nav>

<slot />

<style>
  :global(body) {
    background-color: rgb(58, 84, 71);
    color: rgb(255, 255, 255);
  }

  nav {
    font-family: "Merriweather", serif;
    display: flex;
    justify-content: space-around;
    padding: 0.9rem 0 1.4rem 0;
    border-bottom: 1px solid white;
  }

  nav a {
    font-size: 1.35rem;
    text-decoration: none;
    color: rgb(255, 255, 255);
  }

  nav a:hover {
    text-decoration: underline;
    text-decoration-color: rgb(111, 194, 222);
  }
</style>
