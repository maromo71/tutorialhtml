
# Capítulo 8: APIs no HTML

APIs (Application Programming Interfaces) são conjuntos de ferramentas e protocolos que permitem que diferentes programas interajam entre si. HTML5 introduziu várias APIs que facilitam a criação de aplicações web interativas e dinâmicas.

## 8.1 API de Geolocalização

A API de Geolocalização permite que os aplicativos obtenham a localização do usuário, oferecendo serviços personalizados com base em sua posição.

### Exemplo de Uso

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

## 8.2 API de Arrastar e Soltar

Esta API permite que os desenvolvedores implementem a funcionalidade de arrastar e soltar em suas aplicações web, melhorando a interatividade.

### Exemplo de Uso

```html
<div id="dragItem" draggable="true" ondragstart="drag(event)" style="width:100px;height:100px;background:red;"></div>
<div id="dropZone" ondrop="drop(event)" ondragover="allowDrop(event)" style="width:200px;height:200px;border:1px solid black;"></div>

<script>
  function allowDrop(event) {
    event.preventDefault();
  }

  function drag(event) {
    event.dataTransfer.setData("text", event.target.id);
  }

  function drop(event) {
    event.preventDefault();
    var data = event.dataTransfer.getData("text");
    event.target.appendChild(document.getElementById(data));
  }
</script>
```

## 8.3 API de Web Workers

Web Workers permitem a execução de scripts em segundo plano, sem bloquear a interface do usuário, melhorando o desempenho de aplicações web.

### Exemplo de Uso

```javascript
// worker.js
onmessage = function(event) {
  let result = 0;
  for (let i = 0; i < event.data; i++) {
    result += i;
  }
  postMessage(result);
};

// main script
if (window.Worker) {
  const worker = new Worker('worker.js');
  worker.postMessage(1000000);
  worker.onmessage = function(event) {
    console.log("Resultado: " + event.data);
  };
}
```

## 8.4 WebSocket

WebSockets permitem comunicação bidirecional em tempo real entre o navegador e o servidor, ideal para aplicações como chats e jogos online.

### Exemplo de Uso

```javascript
const socket = new WebSocket('wss://example.com/socket');

socket.onopen = function(event) {
  console.log("Conexão aberta");
  socket.send("Olá, servidor!");
};

socket.onmessage = function(event) {
  console.log("Mensagem do servidor: " + event.data);
};

socket.onclose = function(event) {
  console.log("Conexão fechada");
};
```

## 8.5 Armazenamento na Web

HTML5 introduziu APIs de armazenamento local e de sessão, que permitem armazenar dados diretamente no navegador do usuário.

### Exemplo de Uso

```javascript
// Armazenamento Local
localStorage.setItem('nome', 'Maromo');
console.log(localStorage.getItem('nome'));

// Armazenamento de Sessão
sessionStorage.setItem('sessao', 'Ativa');
console.log(sessionStorage.getItem('sessao'));
```

## 8.6 Eventos Enviados pelo Servidor (Server-Sent Events)

Essa API permite que o servidor envie atualizações automáticas para o navegador, útil para exibir dados em tempo real, como cotações de ações ou resultados esportivos.

### Exemplo de Uso

```javascript
const eventSource = new EventSource('https://example.com/events');

eventSource.onmessage = function(event) {
  console.log("Nova mensagem: " + event.data);
};

eventSource.onerror = function(event) {
  console.error("Erro na conexão");
};
```
