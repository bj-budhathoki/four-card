<script>
  export let title;
  export let text;
  export let icon;
  export let cardType;
</script>

<style>
  .card {
    background: #ffff;
    padding: 30px;
    margin: 15px;
    width: 350px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.05), 0 6px 6px rgba(0, 0, 0, 0.1);
    border-radius: 5px;
    position: relative;
    overflow: hidden;
  }
  .card:nth-child(odd) {
    transform: translateY(50%);
  }
  .card::after {
    content: "";
    position: absolute;
    width: 100%;
    height: 5px;
    top: 0;
    left: 0;
  }
  .red::after {
    background: hsl(0, 78%, 62%);
  }
  .cyan::after {
    background: hsl(180, 62%, 55%);
  }
  .orange::after {
    background: hsl(43, 97%, 64%);
  }
  .blue::after {
    background: hsl(212, 86%, 64%);
  }
  .card h2 {
    margin: 0;
  }
  .card p {
    font-size: 14px;
    margin: 15px 0 30px;
  }
  .card img {
    display: block;
    margin-left: auto;
  }

  @media (max-width: 600px) {
    .card:nth-child(odd) {
      transform: translateY(0%);
    }
  }
</style>

<div class={`card ${cardType}`}>
  <h2>{title}</h2>
  <p>{text}</p>
  <img src={`assets/images/${icon}`} alt={title} />
</div>
