<script>
  let x;
  let y;
  function handleMouseMove(e) {
    console.log(e);
    x = e.clientX - document.documentElement.clientWidth * 1.5;
    y = e.clientY - document.documentElement.clientHeight * 1.5;
  }
</script>

<svelte:window on:mousemove={handleMouseMove} />
<main>
  <button
    ><a href="/posts">
      <div class="button-text">Enter</div>
      <div class="button-text-2">&gt;</div>
    </a></button
  >
  <div class="shadow" style:transform={`translate(${x}px, ${y}px)`} />
</main>

<style>
  button {
    position: absolute;
    z-index: 99;
    padding: 2rem 7rem;
    border: none;
    color: rgb(25, 25, 25);
    margin: 0;
    width: auto;
    overflow: visible;
    font-size: 2rem;
    background: transparent;
    transition: 0.75s;
  }

  button:hover {
    color: rgb(216, 216, 216);
    border: 2px solid rgb(216, 216, 216);
  }

  button:hover a {
    color: rgb(216, 216, 216);
  }

  button:hover .button-text {
    text-decoration: underline;
    text-underline-offset: 3px;
  }

  a {
    display: flex;
    align-items: center;
    gap: 0.7rem;
    color: rgb(216, 216, 216);
    color: rgba(0, 0, 0, 0);
    text-decoration: none;
    transition: 1s;
  }

  .button-text {
    font-family: "Mr Dafoe", cursive;
  }
  .button-text-2 {
    font-size: 2.2rem;
  }

  main {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
    width: 100%;
    position: relative;
    overflow: hidden;
  }
  h1 {
    font-size: 7rem;
    font-family: "Crimson Pro", serif;
    font-weight: 500;
  }

  .shadow {
    position: absolute;
    overflow: hidden;
    cursor: none;
    width: 200vw;
    height: 200vh;
    left: 50%;
    top: 50%;
    transform: translateX(-50%) translateY(-50%);
    background-image: radial-gradient(circle at center, transparent, #000 14%);
  }
</style>
