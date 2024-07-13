<script lang="ts">
  import type { PageData } from "./$types";

  export let data: PageData;
  let products = [
    {
      name: "Product 1",
      prices: [19.99, 29.99, 39.99],
    },
    {
      name: "Product 2",
      prices: [29.99, 39.99, 49.99],
    },
    {
      name: "Product 3",
      prices: [39.99, 49.99, 59.99],
    },
  ];
</script>

<main>
  Prices
  <ul>
    {#each products as { name, prices }}
      <li>{name}</li>
      {#each prices as price}
        <li>{price}</li>
      {/each}
    {/each}
  </ul>
</main>
