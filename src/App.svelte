<script>
  import LinkedIn from "./components/linkedin.svelte";
  import Github from "./components/github.svelte";
  import Mail from "./components/mail.svelte";
</script>

<style>
  main {
    height: 100%;
    text-align: center;
    margin: 0 auto;

    display: flex;
    flex-direction: column;
    align-items: center;
    /* justify-content: center; */
  }

  h1 {
    font-size: 2.5em;
    font-weight: 300;
  }

  h2 {
    font-size: 2em;
    font-weight: 300;

    margin-bottom: 0;
  }

  img {
    border-radius: 100%;
    width: 14em;
  }

  a {
    border-radius: 100%;
    width: 2.75em;
    height: 2.75em;
    border: 1px solid #ff3e00;

    display: flex;
    align-items: center;
    justify-content: center;
  }

  li {
    margin: 0.5em;

    display: inline-block;
    vertical-align: middle;
    position: relative;
  }

  .name {
    color: #ff3e00;
  }

  .label {
    display: none;
  }
</style>

<main>
  <h1>
    Hello, I'm
    <span class="name">Henrique de Castilhos</span>
    .
  </h1>

  <img
    src="https://avatars2.githubusercontent.com/u/35281738?s=460&v=4"
    alt="Henrique de Castilhos" />

  <h2>I'm a software developer.</h2>

  <ul>
    <li>
      <a target="_blank" href="https://linkedin.com/in/henriquedecastilhos">
        <span class="label">LinkedIn</span>
        <LinkedIn />
      </a>
    </li>

    <li>
      <a target="_blank" href="https://github.com/castilh0s">
        <span class="label">GitHub</span>
        <Github />
      </a>
    </li>

    <li>
      <a target="_blank" href="mailto:henrique@castilhos.dev">
        <span class="label">Mail</span>
        <Mail />
      </a>
    </li>
  </ul>
</main>
