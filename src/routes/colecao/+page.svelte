<script>
  let searchQuery = "";

  let products = [
        { id: 1, name: "shorts Lumisoft", price: "R$99,00", img: "https://imagens.liveoficial.com.br/product/750x1125/346602_50658_00BG82_5.jpg" },
        { id: 2, name: "macacão", price: "R$120,00", img: "https://imagens.liveoficial.com.br/product/1000x1500/340346_P1133_00PT01_5.jpg" },
        { id: 3, name: "top cross", price: "R$120,00", img: "https://imagens.liveoficial.com.br/product/1000x1500/361209_O1932_00PT01_5.jpg" },
        { id: 4, name: "macaquinho shorts", price: "R$120,00", img: "https://imagens.liveoficial.com.br/product/1000x1500/340338_P0139_00PT01_5.jpg" },
        { id: 5, name: "top nadador", price: "R$120,00", img: "https://imagens.liveoficial.com.br/product/1000x1500/343951_P1299_0AZ184_5.jpg" },
    ];

$: filteredProducts = products.filter(product =>
        product.name.toLowerCase().includes(searchQuery.toLowerCase())
    );
</script>

<style>
     .search-bar {
        display: flex;
        justify-content: center;
        margin-bottom: 20px;
    }
    .search-input {
        width: 60%;
        padding: 10px;
        border-radius: 5px 0 0 5px;
        border: 2px solid #ff69b4;
        outline: none;
        font-family: Arial, sans-serif;
        font-size: 16px;
    }
    .search-button {
        padding: 10px 20px;
        background-color: #ff69b4;
        border: 2px solid #ff69b4;
        border-radius: 0 5px 5px 0;
        color: white;
        cursor: pointer;
        font-family: Arial, sans-serif;
        font-size: 16px;
        font-weight: bold;
        transition: background-color 0.3s ease;
    }
    .search-button:hover {
        background-color: #ffb6c1;
    }
    
    .product {
        display: inline-block;
        margin: 20px;
        padding: 20px;
        background-color: white;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        border-radius: 8px;
        text-align: center;
    }
    .product img {
        max-width: 200px;
        border-radius: 8px;
    }
    h1 {
        color: #ff69b4;
    }
    p {
        color: #555;
    }
    body {
        font-family: Arial, sans-serif;
        background-color: #fffaf0;
        margin: 0;
        padding: 20px;
        text-align: center;
    }
</style>
<main>

    <h1>Coleção da Live Store</h1>
    <div class="search-bar">
        <input
            type="text"
            class="search-input"
            placeholder="pesquise por coleções.."
            bind:value={searchQuery}
        />
        <button class="search-button" on:click={filteredProducts}>Buscar</button>
    </div>

    {#each filteredProducts as product}
    <div class="product">
        <img src={product.img} alt={product.name}>
        <p>{product.name} - {product.price}</p>
    </div>
{/each}
</main>

<main>
    <h1>Coleção da Live Store</h1>
    <div class="product">
        <img src="https://imagens.liveoficial.com.br/product/750x1125/346602_50658_00BG82_5.jpg" alt="Produto 1">
        <p>shorts Lumisoft - R$99,00</p>
    </div>
    <div class="product">
        <img src="https://imagens.liveoficial.com.br/product/1000x1500/340346_P1133_00PT01_5.jpg" alt="Produto 2">
        <p>macacão - R$120,00</p>
    </div>
    <div class="product">
        <img src="https://imagens.liveoficial.com.br/product/1000x1500/361209_O1932_00PT01_5.jpg" alt="Produto 2">
        <p>top cross - R$120,00</p>
    </div>
    <div class="product">
        <img src="https://imagens.liveoficial.com.br/product/1000x1500/340338_P0139_00PT01_5.jpg" alt="Produto 2">
        <p>macaquinho shorts - R$120,00</p>
    </div>
    <div class="product">
        <img src="https://imagens.liveoficial.com.br/product/1000x1500/343951_P1299_0AZ184_5.jpg" alt="Produto 2">
        <p>top nadado  - R$120,00</p>
    </div>

</main>
