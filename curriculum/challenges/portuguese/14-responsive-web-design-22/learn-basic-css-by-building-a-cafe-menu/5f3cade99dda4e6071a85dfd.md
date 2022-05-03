---
id: 5f3cade99dda4e6071a85dfd
title: Passo 47
challengeType: 0
dashedName: step-47
---

# --description--

Você voltará para o estilo do menu em alguns passos, mas por enquanto, vá em frente e adicione um segundo elemento `section` abaixo do primeiro para exibir as sobremesas oferecidas pela cafeteria.

# --hints--

Você deve acrescentar uma tag de abertura para `section`.

```js
assert(code.match(/<section>/ig).length === 2);
```

Você deve acrescentar uma tag de fechamento para `section`.

```js
assert(code.match(/<\/section>/ig).length === 2);
```

O elemento preexistente `main` deve permanecer o mesmo.

```js
assert($('main').length === 1);
```

O novo elemento `section` deve estar dentro do elemento `main`.

```js
assert($('main').children('section').length === 2);
```

# --seed--

## --seed-contents--

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cafe Menu</title>
    <link href="styles.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <div class="menu">
      <header>
        <h1>CAMPER CAFE</h1>
        <p>Est. 2020</p>
      </header>
      <main>
--fcc-editable-region--
        <section>
          <h2>Coffee</h2>
          <article class="item">
            <p class="flavor">French Vanilla</p><p class="price">3.00</p>
          </article>
          <article class="item">
            <p class="flavor">Caramel Macchiato</p><p class="price">3.75</p>
          </article>
          <article class="item">
            <p class="flavor">Pumpkin Spice</p><p class="price">3.50</p>
          </article>
          <article class="item">
            <p class="flavor">Hazelnut</p><p class="price">4.00</p>
          </article>
          <article class="item">
            <p class="flavor">Mocha</p><p class="price">4.50</p>
          </article>
        </section>
--fcc-editable-region--
      </main>
    </div>
  </body>
<html>
```

```css
body {
  background-image: url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg);
}

h1, h2, p {
  text-align: center;
}

.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
}

.item p {
  display: inline-block;
}

.flavor {
  text-align: left;
  width: 75%;
}

.price {
  text-align: right;
  width: 25%
}
```
