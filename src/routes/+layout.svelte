<script lang="ts">
  import type { LayoutData } from "./$types";

  export let data: LayoutData;
</script>

<main>
  <nav>
    <a href="/">Home</a>
    <a href="/products">Products</a>
    <a href="/about">About</a>
  </nav>
  <slot></slot>

  <div class="footer">&copy; 2024 Your Company. All rights reserved.</div>
</main>

<style>
  /* Assuming you want to apply the gradient to the entire page */
  main {
    min-height: 100vh; /* Make sure it covers the full viewport height */
    width: 100%; /* Cover the full width */
    background: linear-gradient(
      to bottom,
      #e0f7fa 0%,
      #0093e9 50%,
      #80d0c7 100%
    );
    /* This creates a gradient that starts with a light blue at the top,
     transitions to a more vivid blue in the middle,
     and ends with a teal-like color at the bottom */
  }
  nav {
    background-color: #f0f0f0; /* Light grey background */
    padding: 10px 0; /* Padding around the nav */
    text-align: center; /* Center the links */
  }
  nav a {
    color: #333; /* Dark grey text */
    padding: 10px 20px; /* Padding around each link */
    text-decoration: none; /* Remove underline from links */
    font-size: 18px; /* Increase font size */
    margin: 0 10px; /* Space between links */
  }
  nav a:hover {
    background-color: #ddd; /* Light grey background on hover */
    border-radius: 5px; /* Rounded corners on hover */
  }

  .footer {
    margin-top: 3rem;
    font-size: 0.9rem;
  }
</style>
