<script>
  import logo from "./assets/svelte.png";
  import Counter from "./lib/Counter.svelte";
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link
    rel="preconnect"
    href="https://fonts.gstatic.com"
    crossorigin="anonymous"
  />
  <link
    href="https://fonts.googleapis.com/css2?family=Trispace:wght@200;400;700&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<main>
  <div class="header">
    <h1>></h1>
    <h1 class="title">rainqubit</h1>
  </div>
  <div class="content">
    <div class="welcome">
      <p>
        Apple pie carrot cake cake bear claw icing marzipan chupa chups
        chocolate cake tiramisu. Dessert carrot cake oat cake candy canes bonbon
        jelly oat cake lemon drops dessert. Halvah powder jelly beans cake
        halvah icing. Chocolate toffee wafer pudding ice cream jelly-o.
      </p>
    </div>
  </div>
</main>

<style>
  :root {
    font-family: "Trispace", sans-serif;
    font-size: 14px;

    --bg: #000500;
    --fg: #ffffff;
    --primary: #d64045;
    --secondary: #8edce6;

    --s: 0.5rem;
    --m: 1rem;
    --l: 2rem;
    --xl: 4rem;
    --xxl: 8rem;

    background: var(--bg);
    color: var(--fg);
  }

  main {
    text-align: center;
    padding: 0 5% 0 5%;
    margin: 0 auto;
  }

  h1 {
    font-size: var(--l);
  }

  .header {
    display: flex;
    flex-direction: row;
    width: 100%;
    border-bottom: solid 1px;
    border-color: var(--fg);
    margin: 0 0 2rem 0;
  }

  .title {
    font-weight: normal;
    margin-left: 1rem;
  }

  .title::first-letter {
    color: var(--primary);
  }

  .content{
    text-align: justify;
  }

  @media (min-width: 680px) {
    main {
      padding: 0 20% 0 20%;
    }

    .content{
      text-align: left;
    }
  }
</style>
