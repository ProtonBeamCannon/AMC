<script>
  let features = [
    {
      icon: "🚀",
      image: "/amc-content/product1.jpg",
      title: "Fast Performance",
      description: "Easy to use.",
    },
    {
      icon: "🔒",
      image: "/amc-content/info1.jpg",
      title: "Secure",
      description: "Your data is protected with top-notch security measures.",
    },
    {
      icon: "💡",
      image: "/amc-content/product3.jpg",
      title: "Innovative",
      description: "Cutting-edge technology to keep you ahead.",
    },
  ];
</script>

<main>
  <div class="hero">
    <h1>Rumah nyamuk</h1>
    <p>Discover the benefits and features that make our product stand out.</p>
    <a href="/products">Get Started</a>
  </div>

  <div class="features">
    {#each features as feature}
      <div class="feature">
        <div class="icon">{feature.icon}</div>
        <h3>{feature.title}</h3>
        <img src={feature.image} alt="" style="width: 250px; height: 350px;" />
        <p>{feature.description}</p>
      </div>
    {/each}
  </div>
</main>

<style>
  .rotate-90 {
    transform: rotate(90deg);
  }
  main {
    font-family: Arial, sans-serif;
    padding: 2rem;
    text-align: center;
  }
  .hero {
    background-color: #f7f7f7;
    padding: 2rem;
    border-radius: 8px;
  }
  .hero h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
  }
  .hero p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
  }
  .hero button {
    background-color: #0070f3;
    color: white;
    padding: 0.75rem 1.5rem;
    border: none;
    border-radius: 4px;
    font-size: 1rem;
    cursor: pointer;
  }
  .features {
    display: flex;
    justify-content: space-around;
    margin-top: 3rem;
  }
  .feature {
    text-align: center;
    padding: 1rem;
  }
  .feature h3 {
    margin-top: 1rem;
  }
  .footer {
    margin-top: 3rem;
    font-size: 0.9rem;
  }
</style>
