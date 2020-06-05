<script>
  export let title;
  export let text;
  export let icon;
</script>

<div class="card">
  <h3>{title}</h3>
  <p>{text}</p>
  <img src={`assets/images/${icon}`} alt={title} />
</div>
