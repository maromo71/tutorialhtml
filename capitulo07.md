
# Capítulo 7: Gráficos no HTML

HTML oferece suporte a gráficos através de elementos como SVG (Scalable Vector Graphics) e Canvas, permitindo que desenvolvedores criem visuais interativos e dinâmicos em páginas web.

## 7.1 SVG no HTML

SVG é uma linguagem baseada em XML para descrever gráficos vetoriais. Com SVG, você pode criar imagens e formas escaláveis que não perdem qualidade ao serem redimensionadas.

### Exemplo de SVG

```html
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red" />
  <text x="50" y="55" font-size="22" text-anchor="middle" fill="white">SVG</text>
</svg>
```

### Elementos Comuns do SVG

- **`<circle>`**: Define um círculo.
- **`<rect>`**: Define um retângulo.
- **`<line>`**: Define uma linha.
- **`<text>`**: Adiciona texto ao gráfico.

## 7.2 Canvas no HTML

Canvas é um elemento HTML usado para desenhar gráficos por meio de scripts, geralmente em JavaScript. Ele fornece uma área de desenho onde você pode renderizar formas, textos, imagens e animações.

### Exemplo de Canvas

```html
<canvas id="meuCanvas" width="200" height="200" style="border:1px solid #000000;"></canvas>

<script>
  var c = document.getElementById("meuCanvas");
  var ctx = c.getContext("2d");
  ctx.beginPath();
  ctx.arc(100, 100, 50, 0, 2 * Math.PI);
  ctx.stroke();
</script>
```

### Métodos Comuns do Canvas

- **`getContext("2d")`**: Obtém o contexto de desenho 2D.
- **`beginPath()`**: Inicia um novo caminho de desenho.
- **`arc(x, y, raio, início, fim)`**: Desenha um arco ou círculo.
- **`fill()`**: Preenche uma forma com cor.
- **`stroke()`**: Desenha as bordas de uma forma.

## Comparação entre SVG e Canvas

| Característica | SVG | Canvas |
|----------------|-----|--------|
| Modelo         | Vetorial | Bitmap |
| Escalabilidade | Sim, sem perda de qualidade | Não, pode perder qualidade |
| Manipulação    | Baseada em DOM | Baseada em scripts |
| Uso            | Gráficos complexos e estáticos | Animações e gráficos dinâmicos |

## Exemplos Práticos

**SVG: Criando um Retângulo**

```html
<svg width="200" height="100">
  <rect width="100" height="50" style="fill:blue;stroke:black;stroke-width:2;" />
</svg>
```

**Canvas: Desenhando um Retângulo**

```html
<canvas id="meuCanvas2" width="200" height="100"></canvas>

<script>
  var c = document.getElementById("meuCanvas2");
  var ctx = c.getContext("2d");
  ctx.fillStyle = "blue";
  ctx.fillRect(20, 20, 100, 50);
</script>
```
