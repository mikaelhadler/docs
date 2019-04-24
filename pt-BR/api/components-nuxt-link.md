---
title: 'API: O componente <nuxt-link>'
description: Vincule as páginas utilizando o nuxt-link.
---

# O Componente &lt;nuxt-link&gt;

> Este componente é utilizado para vincular os componentes da página entre sí.

No momento, o `<nuxt-link>` é o mesmo que o [`<router-link>`](https://router.vuejs.org/en/api/router-link.html), então nós recomendamos que você veja como usá-lo na [Documentação do Vue Router](https://router.vuejs.org/en/api/router-link.html).

Exemplo (`pages/index.vue`):

```html
<template>
  <div>
    <h1>Página principal</h1>
    <nuxt-link to="/about">Sobre</nuxt-link>
  </div>
</template>
```

No futuro, adicionaremos recursos ao `<nuxt-link>` componente, como pre-fetching em segundo plano para melhorar a capacidade de resposta das aplicações Nuxt.js.
