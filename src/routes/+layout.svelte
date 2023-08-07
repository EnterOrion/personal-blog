<nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/posts">Posts</a>
</nav>

<slot />

<style>
  :global(body) {
    background-color: rgb(11, 11, 11);
    color: rgb(221, 25, 41);
  }

  nav {
    font-family: "Yeseva One", cursive;
    display: flex;
    justify-content: space-around;
  }

  nav a {
    text-decoration: none;
    color: rgb(221, 25, 41);
  }
</style>
