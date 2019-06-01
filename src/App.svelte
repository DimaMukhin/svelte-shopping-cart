<script>
  import Product from "./Product.svelte";

  let title = '';
  let price = '';
  let description = '';

  function setTitle(event) {
      title = event.target.value;
  }
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
    <input type="text" id="title" value="{title}" on:input="{setTitle}" />
  </div>
  <div>
    <label for="price">Price</label>
    <input type="number" id="price" bind:value={price} />
  </div>
  <div>
    <label for="description">Description</label>
    <textarea rows="3" id="description" bind:value={description} />
  </div>
</section>

<Product />
