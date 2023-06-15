<nav>
  <a href="/Tweened">Tweened</a>
  <a href="/Spring">Spring</a>
</nav>

<slot />

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    background-color: #333;
    color: #ccc;
  }

  :global(a) {
    font-size: x-large;
    text-decoration: none;
    color: inherit;
  }

  nav {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    gap: 2vw;
    box-sizing: border-box;
    widows: 100%;
    padding: 0 2vw;
    height: 10vh;
  }
</style>
