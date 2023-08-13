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
    font-family: "Yeseva One", cursive;
    display: flex;
    justify-content: space-around;
  }

  nav a {
    text-decoration: none;
    color: rgb(255, 255, 255);
  }

  nav a:hover {
    text-decoration: underline;
    text-decoration-color: rgb(111, 194, 222);
  }
</style>
