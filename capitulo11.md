
# Capítulo 11: Aplicações de HTML

HTML é uma das linguagens mais utilizadas na web, e suas aplicações são vastas e variadas. Combinado com CSS e JavaScript, HTML forma a base do desenvolvimento web moderno.

## 11.1 Desenvolvimento de Páginas Web

HTML é usado para criar a estrutura de páginas web. Quase todas as páginas na internet contêm HTML em sua base para definir o layout, conteúdo e estrutura.

### Exemplo de Estrutura de Página Web

```html
<!DOCTYPE html>
<html>
<head>
  <title>Minha Página Web</title>
</head>
<body>
  <header>
    <h1>Bem-vindo ao Meu Site</h1>
  </header>
  <nav>
    <ul>
      <li><a href="#home">Início</a></li>
      <li><a href="#about">Sobre</a></li>
      <li><a href="#contact">Contato</a></li>
    </ul>
  </nav>
  <main>
    <section id="home">
      <h2>Início</h2>
      <p>Conteúdo da página inicial.</p>
    </section>
    <section id="about">
      <h2>Sobre</h2>
      <p>Informações sobre o site.</p>
    </section>
    <section id="contact">
      <h2>Contato</h2>
      <p>Formas de entrar em contato conosco.</p>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Meu Site</p>
  </footer>
</body>
</html>
```

## 11.2 UI Responsiva

Com a ajuda de CSS e frameworks como Bootstrap, HTML pode ser usado para criar interfaces de usuário responsivas que funcionam bem em todos os dispositivos, incluindo desktops, tablets e smartphones.

### Exemplo de Responsividade com CSS

```html
<style>
  body {
    font-family: Arial, sans-serif;
  }

  .container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 10px;
  }

  .responsive-image {
    width: 100%;
    height: auto;
  }

  @media (max-width: 600px) {
    .container {
      padding: 5px;
    }
  }
</style>

<div class="container">
  <img src="imagem.jpg" alt="Imagem Responsiva" class="responsive-image">
</div>
```

## 11.3 Desenvolvimento de Jogos

HTML5, com suas capacidades gráficas avançadas, permite o desenvolvimento de jogos diretamente no navegador, usando `<canvas>` para renderização gráfica e JavaScript para lógica de jogo.

### Exemplo Básico de Jogo com Canvas

```html
<canvas id="meuJogo" width="480" height="320"></canvas>

<script>
  const canvas = document.getElementById("meuJogo");
  const context = canvas.getContext("2d");

  function desenhar() {
    context.clearRect(0, 0, canvas.width, canvas.height);
    context.fillStyle = "blue";
    context.fillRect(20, 20, 50, 50);
  }

  setInterval(desenhar, 1000 / 60); // 60 fps
</script>
```

## 11.4 Desenvolvimento de Aplicativos Móveis

Usando HTML, CSS e JavaScript, é possível desenvolver aplicativos móveis híbridos que rodam em múltiplas plataformas usando ferramentas como Apache Cordova ou frameworks como React Native.

## 11.5 Streaming de Multimídia e Vídeo

HTML5 oferece suporte nativo para elementos de vídeo e áudio, permitindo a reprodução de multimídia diretamente no navegador sem plugins adicionais.

### Exemplo de Vídeo HTML5

```html
<video controls>
  <source src="video.mp4" type="video/mp4">
  Seu navegador não suporta o elemento de vídeo.
</video>
```

## 11.6 Geolocalização

HTML5 inclui APIs para acessar a localização geográfica do usuário, o que pode ser usado para fornecer serviços e conteúdo baseados em localização.

### Exemplo de Uso de Geolocalização

```javascript
if (navigator.geolocation) {
  navigator.geolocation.getCurrentPosition(
    function(position) {
      console.log("Latitude: " + position.coords.latitude);
      console.log("Longitude: " + position.coords.longitude);
    },
    function(error) {
      console.error("Erro ao obter localização: ", error);
    }
  );
} else {
  console.log("Geolocalização não é suportada pelo seu navegador.");
}
```
