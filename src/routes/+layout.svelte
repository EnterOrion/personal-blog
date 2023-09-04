<!-- <nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/posts">Posts</a>
</nav> -->

<slot />

<style>
  /* CSS Reset */
  *,
  *::before,
  *::after {
    box-sizing: border-box;
    margin: 0;
  }

  body,
  html {
    height: 100%;
    line-height: 1.5;
    -webkit-font-smoothing: antialiased;
  }

  img,
  picture,
  video,
  canvas,
  svg {
    display: block;
    max-width: 100%;
  }

  input,
  button,
  textarea,
  select {
    font: inherit;
  }

  a {
    text-decoration: none;
  }

  p,
  h1,
  h2,
  h3,
  h4,
  h5,
  h6 {
    overflow-wrap: break-word;
    margin: 0;
    padding: 0;
    border: 0;
    outline: 0;
    font-weight: inherit;
    font-style: inherit;
    font-size: 100%;
    font-family: inherit;
    vertical-align: baseline;
  }

  #root,
  #__next {
    isolation: isolate;
  }

  :global(body) {
    /* background-color: rgb(58, 84, 71); */
    background-color: rgb(25, 25, 25);
    color: rgb(255, 255, 255);
    padding: 0;
    margin: 0;
    height: 100%;
    width: 100%;
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
