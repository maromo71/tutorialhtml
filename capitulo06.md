
# Capítulo 6: Formulários no HTML

Formulários são uma parte crucial da interação do usuário com as páginas web, permitindo a coleta de dados por meio de entradas como texto, botões de seleção, caixas de seleção, e mais.

## 6.1 Formulários HTML

A tag `<form>` define um formulário HTML. Os formulários são usados para enviar dados para um servidor.

```html
<form action="/enviar" method="post">
  <!-- Elementos de entrada do formulário -->
</form>
```

### Atributos Comuns

- **`action`**: Define o destino (URL) para onde os dados do formulário serão enviados.
- **`method`**: Especifica o método HTTP a ser usado ao enviar os dados (`GET` ou `POST`).

## 6.2 Atributos de Formulários

Os atributos do formulário ajudam a controlar o comportamento e a validação dos dados de entrada.

- **`name`**: Identifica um elemento de formulário.
- **`placeholder`**: Mostra um texto de espaço reservado dentro de um campo de entrada.
- **`required`**: Indica que um campo de entrada deve ser preenchido antes de enviar o formulário.

## 6.3 Controle de Formulários

Formulários podem conter vários tipos de controles de entrada:

### Campo de Texto

```html
<label for="nome">Nome:</label>
<input type="text" id="nome" name="nome" placeholder="Digite seu nome" required>
```

### Botões de Rádio

Usados quando apenas uma opção pode ser selecionada entre várias.

```html
<p>Gênero:</p>
<input type="radio" id="masculino" name="genero" value="masculino">
<label for="masculino">Masculino</label>

<input type="radio" id="feminino" name="genero" value="feminino">
<label for="feminino">Feminino</label>
```

### Caixas de Seleção

Usadas quando múltiplas opções podem ser selecionadas.

```html
<p>Interesses:</p>
<input type="checkbox" id="musica" name="interesses" value="musica">
<label for="musica">Música</label>

<input type="checkbox" id="esporte" name="interesses" value="esporte">
<label for="esporte">Esporte</label>
```

### Campos de Seleção (`<select>`)

Oferecem uma lista suspensa de opções.

```html
<label for="pais">País:</label>
<select id="pais" name="pais">
  <option value="brasil">Brasil</option>
  <option value="portugal">Portugal</option>
  <option value="angola">Angola</option>
</select>
```

## 6.4 Atributos de Entrada

Os atributos de entrada permitem personalizar o comportamento e a aparência dos campos de entrada.

- **`type`**: Define o tipo de entrada (ex. `text`, `email`, `password`).
- **`value`**: Define o valor inicial de um campo de entrada.
- **`min` e `max`**: Especificam os limites mínimo e máximo para entradas numéricas.

### Exemplo de Campo Numérico

```html
<label for="idade">Idade:</label>
<input type="number" id="idade" name="idade" min="18" max="99">
```

## Exemplo Completo de Formulário

```html
<form action="/enviar" method="post">
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome" placeholder="Digite seu nome" required>
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Digite seu email" required>
  
  <p>Gênero:</p>
  <input type="radio" id="masculino" name="genero" value="masculino">
  <label for="masculino">Masculino</label>
  <input type="radio" id="feminino" name="genero" value="feminino">
  <label for="feminino">Feminino</label>
  
  <p>Interesses:</p>
  <input type="checkbox" id="musica" name="interesses" value="musica">
  <label for="musica">Música</label>
  <input type="checkbox" id="esporte" name="interesses" value="esporte">
  <label for="esporte">Esporte</label>
  
  <input type="submit" value="Enviar">
</form>
```
