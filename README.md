O projeto de que estou fazendo e sobre um site para um escritorio de advocacia.
Nesse projeto temos as seguintes paginas: PAgina inicial, Paginas formularia dos clientes, sobre os advogados entre outros
Aqui tem uns codigos como exemplo que usei no meu codigo:


Pagina inicial:
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Escritório de Advocacia</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f6f6f6;
        }
        header {
            background-color: #707288;
            color: rgb(255, 255, 255);
            padding: 15px 0;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #90908cbc;
            padding: 10px;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .content {
            padding: 20px;
        }
        section {
            margin: 20px 0;
        }
        footer {
            background-color: #929292;
            color: rgb(7, 7, 7);
            text-align: center;
            padding: 10px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        h2 {
            color: #c8c8c8;
        }
        p {
            color: #242121;
            line-height: 1.6;
        }
    </style>
</head>
<body>

<header>
    <h1>Bem-vindo ao Nosso Escritório de Advocacia</h1>
</header>

<nav>
    <a href="Sitesobrenos.html">Sobre nos</a>
    <a href="formulariodoclientenosite.html">Clientes</a>
    <a href="siteareadeatuação.html">Áreas de Atuação</a>
    <a href="sitehistoriadoescritorio.html">História do Escritório</a>
    <a href="siteadvogados.html">Advogados</a>
    <a href="siteservicos.html">Serviços</a>
    <a href="siteajuda.html">Como Podemos Ajudar</a>
    <a href="imagem.html"> Onde pode nos encontrarmos</a>
</nav>

<footer>
    <p>&copy; 2024 Escritório Del Padre Advocacia. Todos os direitos reservados.</p>
</footer>

</body>
</html>


Paginas do formulario dos clientes
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Escritório de Advocacia</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header></header>
    <div class="logo">
      <img src="IMG-20240919-WA0007" alt="Logo do Escritório">
    </div>

   <section id="home">
    <h1>Bem-vindo ao Nosso Escritório de Advocacia</h1>
    <p>Atuamos com dedicação e comprometimento nas principais áreas do direito, garantindo aos nossos clientes excelência na prestação de serviços jurídicos.</p>
   
  </section>

  <section id="sobre-nos"></section>
    <h2>Sobre Nós</h2>
    <p>Com anos de experiência, nosso escritório se destaca pela confiança, ética e eficiência no atendimento aos nossos clientes.</p>
  </section>
 
  <section id="areas"></section>
    <h2>Áreas de Atuação</h2>
    <ul>
        <li><a href="">Direito Civil </a></li>
        <li><a href="">Direito Trabalhista</a></li>
        <li><a href="">Direito do Consumidor</a></li>
        <li><a href="">Direito Predvidenciario</a></li>
        <li><a href="">Direito Digital</a></li>
    </ul>
  </section>

  <section id="contato"> </section>
    <h2>Informações:</h2>
    <nav>
      <ul> 
        <li><a href="">Home</a></li>
        <li><a href="">Sobre Nós</a></li>
        <li><a href="">Serviços</a></li>
        <li><a href="">Contato</a></li>
      </ul>
    </nav>
  </header>
    <h1>Dados necessesario:</h1>

    <form action="envio.php" method="post">
      <label for="nome">Nome:</label>
      <input type="text" id="nome" name="nome" required>
      <br><br>
    
      <form action="#">
        <label for="numerodetelefone">Adicione seu numero de telefone:</label>
        <input type="tel" id="numero" name="numerodetelefone"
        placeholder="(xx) xxxxx-xxxx"
        pattern="\([0-9]{2}\)[\s][0-9]{4,5}-[0-9]{4}" /">
      <br><br>
    
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>
      <br><br>
    
      <h3>Enderço:</h3>
      <label for="rua">Rua:</label>
      <input type="rua" id="rua" name="rua" required>
      <br><br>
    
      <label for="bairro">Bairro:</label>
      <input type="bairro" id="bairro" name="bairro" required>
      <br><br>
    
      <label for="numero">Numero:</label>
      <input type="numero" id="numero" name="numero" required>
      <br><br><br>

      <h3> Caso:</h3>
      <label for="tipodecaso">Tipo de caso:</label>
      <select id="tipodecaso" name="tipodecaso" required>
        <option value="direito-civil">Direito Civil</option>
        <option value="direito-trabalhista">Direito Trabalhista</option>
        <option value="direito-penal">Direito do Consumidor</option>
        <option value="direito-empresarial">Direito Predvidenciario </option>
        <option value="direito-civil">Direito Digital</option>
      </select>
      <br><br>
    
      <label for="descricaodocaso">Descrição do caso:</label>
      <textarea id="descricaodocaso" name="descricaodocaso" rows="5" cols="33" placeholder="Descreva o caso detalhadamente" required></textarea>
      <br><br>
    
      <label for="datadoincidente">Data do incidente:</label>
      <input type="date" id="datadoincidente" name="datadoincidente" required>
      <br><br>
    
      <label for="partasenvolvidas">Partas envolvidas:</label>
      <input type="text" id="partasenvolvidas" name="partasenvolvidas" placeholder="Nome das partes envolvidas" required>
      <br><br>
      
      <label for="uploaddedocumentos">Upload de Documentos (PDF, JPG, etc.):</label>
      <input type="file" id="uploaddedocumentos" name="uploaddedocumentos[]" accept=".pdf, .jpg, .png" multiple required>
      <br><br>
    
      <label for="objetivo">Objetivo:</label>
      <input type="text" id="objetivo" name="objetivo" placeholder="Qual é o seu objetivo com esse caso?" required>
      <br><br>

      <label for="orcamento">Orçamento:</label>
      <input type="number" id="orcamento" name="orcamento" placeholder="Valor aproximado" min="0" step="5.00" required>
      <br><br>

      <button type="submit">Enviar</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2024 Escritório del padre Advocacia. Todos os direitos reservados.</p>
  </footer>

</body>
</html>

Parte dos advogados
    <section id="advogados">
        <h2>Nossos Advogados</h2>
        <p>Contamos com uma equipe de advogados experientes e altamente qualificados, especializados em diversas áreas do direito. Nosso time está comprometido em oferecer um atendimento dedicado e soluções jurídicas eficientes.</p>
    </section>

