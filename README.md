# Edouk
site de vendas para e-books 
meu-ebook-site/
│
├── index.html
├── style.css
└── script.js
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Loja de E-books</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>📚 Ebooks Digitais</h1>
    <nav>
      <a href="#">Início</a>
      <a href="#">Categorias</a>
      <a href="#">Contato</a>
    </nav>
  </header>

  <main>
    <h2>Mais vendidos</h2>
    <section class="ebook-list">
      <div class="ebook">
        <img src="https://via.placeholder.com/150" alt="E-book 1">
        <h3>E-book: Aprenda a Programar</h3>
        <p>R$ 29,90</p>
        <button onclick="comprar('Aprenda a Programar')">Comprar</button>
      </div>
      <div class="ebook">
        <img src="https://via.placeholder.com/150" alt="E-book 2">
        <h3>E-book: Finanças Pessoais</h3>
        <p>R$ 24,90</p>
        <button onclick="comprar('Finanças Pessoais')">Comprar</button>
      </div>
      <!-- Adicione mais e-books aqui -->
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Loja de E-books. Todos os direitos reservados.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background-color: #f9f9f9;
  color: #333;
}

header {
  background-color: #4a90e2;
  color: white;
  padding: 20px;
  text-align: center;
}

nav a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
}

main {
  padding: 20px;
}

.ebook-list {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}

.ebook {
  background-color: white;
  border: 1px solid #ccc;
  border-radius: 8px;
  width: 200px;
  padding: 15px;
  text-align: center;
}

.ebook img {
  width: 100%;
  border-radius: 4px;
}

button {
  background-color: #4a90e2;
  color: white;
  border: none;
  padding: 10px;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #357ABD;
}

footer {
  text-align: center;
  padding: 10px;
  background-color: #eee;
}
function comprar(titulo) {
  alert(`Você comprou o e-book: ${titulo}!\nEm breve você receberá no seu e-mail.`);
}
