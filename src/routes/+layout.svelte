<nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/posts">Posts</a>
</nav>

<slot />

<style>
  :global(body) {
    background-color: rgb(53, 49, 49);
    color: rgb(222, 222, 222);
  }

  nav {
    font-family: "Yeseva One", cursive;
    display: flex;
    justify-content: space-around;
  }

  nav a {
    text-decoration: none;
    color: rgb(222, 222, 222);
  }
</style>
