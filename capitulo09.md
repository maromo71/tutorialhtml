
# Capítulo 9: Referências de HTML

Referências de HTML são recursos essenciais que fornecem informações detalhadas sobre tags, atributos, eventos, fontes e muito mais. Essas referências são úteis tanto para desenvolvedores iniciantes quanto para os mais experientes.

## 9.1 Referência de Tags

A referência de tags HTML lista todas as tags disponíveis, suas descrições e exemplos de uso. Aqui estão algumas das tags mais comuns:

- **`<a>`**: Define um hyperlink.
- **`<div>`**: Define uma divisão ou seção em um documento.
- **`<span>`**: Define uma seção em linha usada para agrupar elementos.
- **`<img>`**: Define uma imagem.
- **`<form>`**: Define um formulário HTML.

## 9.2 Referência de Atributos

Os atributos HTML fornecem informações adicionais sobre elementos. Aqui estão alguns atributos comuns:

- **`class`**: Especifica uma ou mais classes para um elemento, usadas por CSS e JavaScript.
- **`id`**: Especifica um identificador único para um elemento.
- **`src`**: Especifica a URL de uma imagem ou recurso.
- **`alt`**: Fornece um texto alternativo para imagens.
- **`style`**: Aplica estilos CSS diretamente a um elemento.

## 9.3 Referência de Eventos

Os eventos HTML permitem que scripts respondam a ações do usuário ou mudanças de estado do documento. Exemplos de eventos incluem:

- **`onclick`**: Disparado quando um elemento é clicado.
- **`onchange`**: Disparado quando o valor de um elemento muda.
- **`onmouseover`**: Disparado quando o cursor do mouse passa sobre um elemento.
- **`onload`**: Disparado quando um documento ou imagem termina de carregar.

## 9.4 Referência de Fontes

As fontes HTML referem-se aos estilos de texto que podem ser aplicados usando CSS. Exemplos de propriedades de fontes incluem:

- **`font-family`**: Define a fonte do texto.
- **`font-size`**: Define o tamanho do texto.
- **`font-weight`**: Define a espessura do texto (normal, bold, etc.).
- **`font-style`**: Define o estilo do texto (normal, italic, etc.).

## Exemplos Práticos

**Uso de Atributos e Eventos:**

```html
<button id="meuBotao" class="btn" onclick="alert('Você clicou no botão!')">Clique aqui</button>

<img src="imagem.jpg" alt="Descrição da imagem" onmouseover="this.style.border='2px solid blue'">
```

**Aplicando Fontes com CSS:**

```html
<style>
  .texto-personalizado {
    font-family: 'Arial', sans-serif;
    font-size: 16px;
    font-weight: bold;
    color: #333;
  }
</style>

<p class="texto-personalizado">Este é um texto com estilo personalizado.</p>
```

## Recursos de Referência Online

- **[MDN Web Docs](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element)**: Uma das referências mais completas e confiáveis para HTML e outras tecnologias web.
- **[W3Schools HTML Reference](https://www.w3schools.com/tags/default.asp)**: Um recurso popular para iniciantes com exemplos interativos.
- **[HTML Reference](https://htmlreference.io/)**: Um guia visual que lista todas as tags HTML.
