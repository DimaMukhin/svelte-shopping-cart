<script>
  import Product from "./Product.svelte";

  export let name;
</script>

<style>
  section {
      width: 30rem;
      margin: auto;
  }

  label,
  input,
  textarea {
      width: 100%;
  }
</style>

<section>
  <div>
    <label for="title">Title</label>
    <input type="text" id="title" />
  </div>
  <div>
    <label for="price">Price</label>
    <input type="number" id="price" />
  </div>
  <div>
    <label for="description">Description</label>
    <textarea rows="3" id="description" />
  </div>
</section>

<Product />
