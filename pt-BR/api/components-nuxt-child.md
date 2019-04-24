---
title: 'API: Componente <nuxt-child> '
description: Exibe a página atual.
---

# O Componente &lt;nuxt-child&gt;

> Este componente é usado para exibir os componentes filhos em uma [Nested Routes](/guide/routing#nested-routes).

Exemplo:

```bash
-| pages/
---| parent/
------| child.vue
---| parent.vue
```

Esta árvore de arquivos irá gerar essas rotas:

```js
;[
  {
    path: '/parent',
    component: '~/pages/parent.vue',
    name: 'parent',
    children: [
      {
        path: 'child',
        component: '~/pages/parent/child.vue',
        name: 'parent-child'
      }
    ]
  }
]
```

Para exibir o component `child.vue`, temos que inserir o `<nuxt-child/>` dentro de `pages/parent.vue`:

```html
<template>
  <div>
    <h1>Eu sou a view pai</h1>
    <nuxt-child />
  </div>
</template>
```

Para ver um exemplo, dê uma olhada no [exemplo de nested-routes](/examples/nested-routes).
