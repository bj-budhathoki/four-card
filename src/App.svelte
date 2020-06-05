<script>
  import Card from "./components/Card.svelte";
  import Footer from "./layouts/Footer.svelte";
</script>

<style>
  header {
    margin: 50px auto;
    max-width: 500px;
    text-align: center;
  }
  h1 {
    font-weight: 200;
    margin: 0;
  }
  span {
    font-weight: 500;
  }
  p {
    color: hsl(229, 6%, 66%);
  }
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
    max-width: 1140px;
    flex-wrap: wrap;
  }
</style>

<main>
  <header>
    <h1>
      Reliable, efficinet delivery
      <span>Powered by Technology</span>
    </h1>
    <p>
      Our Artificial intelligence powered tools use millions of project data
      points to ensure that your project issuccessful.
    </p>
  </header>
  <div class="container">
    <Card
      title="Supervisor"
      text="Monitors activity to identify project roadblocks"
      icon="icon-supervisor.svg"
      cardType="cyan" />

    <Card
      title="Team Builder"
      text="Scans our talent network to create the optimal team for your
      project."
      icon="icon-team-builder.svg"
      cardType="red" />

    <Card
      title="Karmas"
      text="Regularly evaluates our talent to ensure quality"
      icon="icon-karma.svg"
      cardType="orange" />

    <Card
      title="Calculator"
      text="Uses data from past projects to provide better delivery estimates"
      icon="icon-calculator.svg"
      cardType="blue" />
  </div>
  <!-- <Footer /> -->
</main>
