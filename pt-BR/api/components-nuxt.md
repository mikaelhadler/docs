---
title: 'API: O componente <nuxt>'
description: Exibe os components da página dentro de um layout.
---

# O Componente &lt;nuxt&gt;

> Este componente é usado somente em [layouts](/guide/views#layouts) para exibir os components da página.

**Propriedades**:

- nuxtChildKey: `string`
  - Esta propriedade vai ser configurada para `<router-view/>`, utilizada para fazer transições dentro de uma página dinâmica e rota diferente.
  - Padrão: `$route.fullPath`

Exemplo (`layouts/default.vue`):

```html
<template>
  <div>
    <div>Meu nav bar</div>
    <nuxt />
    <div>Meu footer</div>
  </div>
</template>
```

Para ver um exemplo, dê uma olhada nos [exemplos de layout](/examples/layouts).
