<!-- <nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/posts">Posts</a>
</nav> -->

<slot />

<style>
  :global(body) {
    /* background-color: rgb(58, 84, 71); */
    background-color: rgb(25, 25, 25);
    color: rgb(255, 255, 255);
    height: 100vh;
    width: 100vw;
    padding: 0;
    margin: 0;
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
    color: rgb(222, 222, 222);
  }
</style>
