
# Capítulo 5: Links no HTML

Links, ou hiperlinks, são um dos componentes fundamentais da web, permitindo a navegação entre páginas e recursos. Com HTML, você pode criar links para outras páginas, imagens, emails, e muito mais.

## 5.1 Links de Texto

A tag `<a>` é usada para criar links em HTML. O atributo `href` especifica o destino do link.

```html
<a href="https://www.exemplo.com">Visite nosso site</a>
```

### Atributos Comuns

- **`href`**: Define o destino do link.
- **`target`**: Determina onde o link será aberto (`_blank` para nova aba/janela, `_self` para a mesma aba/janela).

```html
<a href="https://www.exemplo.com" target="_blank">Abrir em nova aba</a>
```

## 5.2 Links de Imagem

Links também podem ser aplicados a imagens, permitindo que o usuário clique na imagem para navegar para um destino.

```html
<a href="https://www.exemplo.com">
  <img src="imagem.jpg" alt="Imagem Exemplo">
</a>
```

## 5.3 Links de Email

A tag `<a>` pode ser usada para criar links de email, que abrirão o cliente de email padrão do usuário com um novo email já endereçado.

```html
<a href="mailto:contato@exemplo.com">Envie-nos um email</a>
```

## Exemplos Práticos

### Exemplo de Link de Texto:

```html
<a href="https://www.wikipedia.org">Wikipedia</a>
```

### Exemplo de Link de Imagem:

```html
<a href="https://www.wikipedia.org">
  <img src="logo.png" alt="Wikipedia Logo">
</a>
```

### Exemplo de Link de Email:

```html
<a href="mailto:info@empresa.com">Contate-nos</a>
```

## Práticas Recomendas

- Sempre use o atributo `alt` para imagens em links, para acessibilidade.
- Verifique se o texto do link é descritivo para que os usuários saibam para onde estão navegando.

## Usando âncoras para navegação dentro da mesma página

Você pode criar âncoras para permitir que os usuários naveguem para diferentes partes da mesma página.

```html
<!-- Link de navegação -->
<a href="#section1">Ir para a Seção 1</a>

<!-- Destino da âncora -->
<h2 id="section1">Seção 1</h2>
<p>Conteúdo da seção 1...</p>
```
