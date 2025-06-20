<!DOCTYPE html><html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Complexo Escolar Privado Fulama - Educação de Excelência</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Inter:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --luxo: #c5a265;
      --claro: #ffffff;
      --escuro: #111111;
      --cinza: #f0f0f0;
      --texto-dark: #eeeeee;
      --azul: #004aad;
      --dourado: #d4af37;
    }* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', sans-serif;
  background: var(--claro);
  color: var(--escuro);
  transition: background 0.4s, color 0.4s;
  line-height: 1.6;
}

.dark-mode {
  background: #1a1a1a;
  color: var(--texto-dark);
}

header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: var(--escuro);
  color: var(--claro);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  z-index: 1000;
}

header h1 {
  font-family: 'Playfair Display', serif;
  color: var(--dourado);
  font-size: 1.7rem;
}

nav {
  display: flex;
  gap: 1.5rem;
}

nav a {
  color: var(--claro);
  text-decoration: none;
  font-weight: 500;
}

nav a:hover {
  color: var(--dourado);
}

.btn-darkmode {
  background: none;
  border: 1px solid var(--dourado);
  padding: 6px 14px;
  border-radius: 20px;
  color: var(--dourado);
  cursor: pointer;
}

.menu-toggle {
  display: none;
  flex-direction: column;
  cursor: pointer;
}

.menu-toggle div {
  width: 25px;
  height: 3px;
  background: var(--claro);
  margin: 4px 0;
}

@media (max-width: 768px) {
  nav {
    display: none;
    flex-direction: column;
    background: var(--escuro);
    position: absolute;
    top: 60px;
    right: 20px;
    padding: 1rem;
    border-radius: 10px;
  }
  nav.active {
    display: flex;
  }
  .menu-toggle {
    display: flex;
  }
}

.hero {
  padding-top: 6rem;
  background: linear-gradient(to right, #002244, #004aad);
  color: var(--claro);
  text-align: center;
  padding: 8rem 2rem;
  position: relative;
}

.hero::after {
  content: "";
  position: absolute;
  bottom: -30px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 6px;
  background: var(--dourado);
  border-radius: 10px;
}

.hero h2 {
  font-family: 'Playfair Display', serif;
  font-size: 2.8rem;
}

.hero p {
  font-size: 1.2rem;
  margin-top: 1rem;
  color: #eee;
}

.section {
  padding: 4rem 2rem;
  max-width: 1200px;
  margin: auto;
  text-align: center;
}

.section h3 {
  font-family: 'Playfair Display', serif;
  font-size: 2rem;
  margin-bottom: 2rem;
  color: var(--azul);
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.card {
  background: var(--claro);
  padding: 2rem;
  border-radius: 1rem;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.07);
  transition: transform 0.3s, background 0.3s;
}

.dark-mode .card {
  background: #2a2a2a;
}

.card:hover {
  transform: translateY(-6px);
}

footer {
  background: var(--escuro);
  color: #ccc;
  text-align: center;
  padding: 2rem;
  margin-top: 3rem;
}

  </style>
</head>
<body>
  <header>
    <h1>Complexo Escolar Privado Fulama</h1>
    <div class="menu-toggle" onclick="toggleMenu()">
      <div></div><div></div><div></div>
    </div>
    <nav id="menu">
      <a href="#cursos">Cursos</a>
      <a href="#sobre">Sobre</a>
      <a href="#contato">Contato</a>
      <button class="btn-darkmode" onclick="alternarTema()">Modo</button>
    </nav>
  </header>  <section class="hero">
    <h2>Educação de Excelência<br>para o Futuro</h2>
    <p><strong>Transformando vidas com ensino de alta qualidade,<br>estrutura de ponta e inovação pedagógica.</strong></p>
  </section>  <section class="section" id="cursos">
    <h3>Nossos Cursos</h3>
    <div class="cards">
      <div class="card">
        <h4>Educação Infantil</h4>
        <p>Ambiente seguro e criativo para o desenvolvimento cognitivo e emocional das crianças.</p>
      </div>
      <div class="card">
        <h4>Ensino Fundamental</h4>
        <p>Formação sólida com foco no conhecimento, valores e construção de caráter.</p>
      </div>
      <div class="card">
        <h4>Ensino Médio</h4>
        <p>Preparação completa para vestibulares, ENEM e desafios acadêmicos do futuro.</p>
      </div>
    </div>
  </section>  <section class="section" id="sobre">
    <h3>Sobre a Instituição</h3>
    <p>O Complexo Escolar Privado Fulama é referência em educação de alto padrão,<br>combinando tecnologia, tradição e humanização. Nossos professores são líderes<br>em suas áreas e a estrutura foi pensada para maximizar o aprendizado.</p>
  </section>  <section class="section" id="contato">
    <h3>Fale Conosco</h3>
    <p>Telefone: (+224) 953-396-094<br>📍 Av. das Nações, 1000 - Cidade Educacional</p>
  </section>  <footer>
    &copy; 2025 Complexo Escolar Privado Fulama - Todos os direitos reservados.
  </footer>  <script>
    function alternarTema() {
      document.body.classList.toggle("dark-mode");
    }

    function toggleMenu() {
      document.getElementById("menu").classList.toggle("active");
    }

    // Animações suaves ao rolar
    window.addEventListener('scroll', () => {
      document.querySelectorAll('.card').forEach(card => {
        const rect = card.getBoundingClientRect();
        if(rect.top < window.innerHeight - 50){
          card.style.transition = 'transform 0.6s ease, opacity 0.6s';
          card.style.opacity = 1;
          card.style.transform = 'translateY(0)';
        }
      });
    });

    // Inicialização
    document.querySelectorAll('.card').forEach(card => {
      card.style.opacity = 0;
      card.style.transform = 'translateY(50px)';
    });
  </script></body>
</html>
