<script>
  // export let name;
  // let name='adam'
  let src = "";
  let name = "rickrolled";
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }

    p {
      color: blue;
      font-family: "Times New Roman", Times, cursive;
      font-size: 5em;
    }
  }
</style>

<main>
  <h1>Hello {name}!</h1>
  <img {src} alt="{name} :)" />
  <p>
    Visit the
    <a href="https://svelte.dev/tutorial">Svelte tutorial</a>
    to learn how to build Svelte apps.
  </p>
</main>
