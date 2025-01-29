<script>
    let message = "Bem-vindo à Live Store, sua loja de roupas virtuais!";
    function changeBackgroundColor() {
        document.body.style.backgroundColor = '#e0f7fa'; 
    }
</script>

<style>
    .nav-link {
        text-decoration: none;
        color: #ff69b4; 
        font-weight: bold;
        padding: 10px 20px;
        border-radius: 5px;
        transition: background-color 0.3s ease, color 0.3s ease;
    }
    .nav-link:hover {
        background-color: #ffb6c1; 
        color: #ffffff;
    }
    body {
        font-family: 'Comic Sans MS', cursive, sans-serif; 
        background-color: #fffaf0;
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
    }
    .container {
        text-align: center;
        background: white;
        padding: 20px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        border-radius: 8px;
        border: 2px solid #ff69b4; 
    }
    h1 {
        color: #ff69b4;
    }
    p {
        color: #555;
    }
    .button {
        margin-top: 20px;
        padding: 10px 20px;
        background-color: #ff69b4;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-weight: bold;
    }
    .button:hover {
        background-color: #ffb6c1;
    }
</style>

<main>
    <div class="container">
        <h1>{message}</h1>
        <p>Explore nossa coleção e descubra as últimas tendências da moda!</p>
        <button class="button" on:click={() => alert('Seja bem-vindo à Live Store!')}>Clique aqui</button>
        <button class="button" on:click={changeBackgroundColor}>Altere para azul</button>
        <nav>
            <a class="nav-link" href="colecao">Coleção</a>
            <a class="nav-link" href="promocao">Promoções</a>
        </nav>
    </div>
</main>
