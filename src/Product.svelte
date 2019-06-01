<script>
    export let productTitle;
    export let productDescription;
    export let productPrice;
</script>

<style>
    div {
        margin: 1rem;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.26);
        padding: 1rem;
        border-radius: 5px;
        background: white;
    }

    h1 {
        font-size: 1.25rem;
        margin: 0.25rem 0;
    }

    h2 {
        font-size: 1rem;
        margin: 0.25rem 0;
        color: #4b4b4b;
    }

    p {
        margin: 0.25rem 0;
    }

    button {
        font: inherit;
        padding: 0.15rem 0.5rem;
        background: #b10057;
        border: 1px solid #b10057;
        color: white;
        cursor: pointer;
    }

    button:hover,
    button:active {
        box-shadow: 1px 1px 6px rgba(0, 0, 0, 0.26);
    }
</style>

<div>
    <h1>{productTitle}</h1>
    <h2>{productPrice}</h2>
    <p>{productDescription}</p>
    <button>Add to Cart</button>
</div>