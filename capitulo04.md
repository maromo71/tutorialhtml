
# Capítulo 4: Tabelas no HTML

Tabelas são usadas para organizar dados em linhas e colunas, facilitando a apresentação de informações estruturadas. HTML oferece diversas tags para criar e estilizar tabelas.

## 4.1 Tag `<table>`

A tag `<table>` é usada para definir uma tabela. Dentro dessa tag, você pode criar linhas, cabeçalhos e células de dados.

```html
<table>
  <!-- Linhas e células da tabela serão inseridas aqui -->
</table>
```

## 4.2 Tags `<thead>` e `<tbody>`

- **`<thead>`**: Usada para agrupar o conteúdo de cabeçalhos de uma tabela. Normalmente contém `<tr>` com `<th>`.
- **`<tbody>`**: Usada para agrupar o corpo do conteúdo da tabela. Contém `<tr>` com `<td>`.

```html
<table>
  <thead>
    <tr>
      <th>Nome</th>
      <th>Idade</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Ana</td>
      <td>30</td>
    </tr>
    <tr>
      <td>João</td>
      <td>25</td>
    </tr>
  </tbody>
</table>
```

## 4.3 Tag `<tr>`

A tag `<tr>` define uma linha em uma tabela. Pode conter `<th>` (cabeçalhos) ou `<td>` (dados).

## 4.4 Tag `<th>`

A tag `<th>` define um cabeçalho de célula em uma tabela. O conteúdo é geralmente exibido em negrito e centralizado.

```html
<tr>
  <th>Produto</th>
  <th>Preço</th>
</tr>
```

## 4.5 Tag `<td>`

A tag `<td>` define uma célula de dados em uma tabela.

```html
<tr>
  <td>Caneta</td>
  <td>R$ 2,00</td>
</tr>
```

## 4.6 Cabeçalhos e Legendas

- **Cabeçalhos**: Usados para descrever colunas, através de `<th>`.
- **Legenda (`<caption>`)**: Fornece uma descrição para a tabela, geralmente posicionada no topo.

```html
<table>
  <caption>Lista de Produtos</caption>
  <tr>
    <th>Produto</th>
    <th>Preço</th>
  </tr>
  <tr>
    <td>Lápis</td>
    <td>R$ 1,00</td>
  </tr>
</table>
```

## 4.7 Estilização de Tabelas

Estilos podem ser aplicados às tabelas usando CSS para melhorar a apresentação visual. Exemplos incluem adicionar bordas, alterar cores de fundo e definir espaçamentos.

```html
<style>
  table {
    width: 100%;
    border-collapse: collapse;
  }
  th, td {
    border: 1px solid #ccc;
    padding: 8px;
    text-align: left;
  }
  th {
    background-color: #f2f2f2;
  }
</style>
```

## 4.8 Colunas de Grupo (`<colgroup>`)

A tag `<colgroup>` é usada para definir grupos de colunas em uma tabela, permitindo aplicar estilos específicos a colunas inteiras.

```html
<table>
  <colgroup>
    <col style="background-color: #f2f2f2">
    <col style="background-color: #e6e6e6">
  </colgroup>
  <tr>
    <th>Nome</th>
    <th>Idade</th>
  </tr>
  <tr>
    <td>Maria</td>
    <td>22</td>
  </tr>
</table>
```

## 4.9 Tabelas Aninhadas

Tabelas podem ser aninhadas dentro de células de outras tabelas, embora isso deva ser usado com cuidado para não complicar demais a estrutura da página.

```html
<table border="1">
  <tr>
    <td>
      <table border="1">
        <tr>
          <td>Aninhada 1</td>
        </tr>
      </table>
    </td>
    <td>Principal</td>
  </tr>
</table>
```
