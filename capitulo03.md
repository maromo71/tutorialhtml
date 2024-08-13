
# Capítulo 3: Listas no HTML

Listas são uma maneira de agrupar itens relacionados em uma página web. HTML oferece suporte a vários tipos de listas que podem ser usadas para organizar e apresentar informações de maneira clara e estruturada.

## 3.1 Listas Ordenadas e Não Ordenadas

### Listas Ordenadas (`<ol>`)

Listas ordenadas são usadas para exibir itens em uma sequência numerada. A tag `<ol>` cria uma lista ordenada.

```html
<ol>
  <li>Primeiro item</li>
  <li>Segundo item</li>
  <li>Terceiro item</li>
</ol>
```

### Listas Não Ordenadas (`<ul>`)

Listas não ordenadas são usadas para exibir itens em uma sequência sem ordem específica, geralmente com marcadores. A tag `<ul>` cria uma lista não ordenada.

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

## 3.2 Tag `<li>`

A tag `<li>` é usada para definir um item de lista, seja em uma lista ordenada ou não ordenada. Cada item em uma lista é representado por `<li>`.

```html
<ul>
  <li>Primeiro item</li>
  <li>Segundo item</li>
</ul>
```

## 3.3 Listas de Definição

Listas de definição são usadas para exibir pares de termos e suas descrições, como glossários ou FAQs.

### Tag `<dl>`

A tag `<dl>` define uma lista de definições.

```html
<dl>
  <dt>HTML</dt>
  <dd>Hypertext Markup Language</dd>
  
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```

### Tag `<dt>`

A tag `<dt>` é usada para definir um termo na lista de definições.

### Tag `<dd>`

A tag `<dd>` é usada para fornecer a descrição ou definição do termo.

## Exemplos Práticos

### Exemplo de Lista Ordenada:

```html
<ol>
  <li>Comprar ingredientes</li>
  <li>Preparar a massa</li>
  <li>Assar o bolo</li>
</ol>
```

### Exemplo de Lista Não Ordenada:

```html
<ul>
  <li>Maçãs</li>
  <li>Bananas</li>
  <li>Uvas</li>
</ul>
```

### Exemplo de Lista de Definição:

```html
<dl>
  <dt>JavaScript</dt>
  <dd>Uma linguagem de programação para a web.</dd>
  
  <dt>HTML</dt>
  <dd>A linguagem de marcação para criar páginas web.</dd>
</dl>
```
