---
theme: apple-basic
layout: statement
title: Storybook
---

<style>
h1 {
    display: inline-block;
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    background-image: linear-gradient(90deg,#2ca2b4,#5598de 24%,#7f87ff 45%,#f65aad 76%,#ec3d43);
    will-change: transform;
    padding-top: .5px;
    overflow: hidden;
    background-color: #2ca2b4 0%;
    margin-top: 14px;
    padding: 10px;
    
}

.image-cover {
  display: flex;
  justify-content: center;

}
.img-cover {
  width: 150px;
}

.img-ss {
  width: 700px;
}
</style>
# Storybook
<div class=image-cover>
<img class=img-cover src="https://res.cloudinary.com/lesteban/image/upload/v1666829094/Logos/storybook-icon_xbqgkj.svg" >
</div>
---
layout: bullets
---
# ¿Qué es?

 * Herramienta que sirve para crear componentes visuales de forma aislada
 * Sirve Para React - Vue - Angular 
 * Te permite trabajar un componente a la vez
  
---
layout: bullets
---
# ¿Para qué sirve?

* Te permite documentar los componentes de la aplicación para su reutilización
* Realizar pruebas visuales automáticas para evitar errores.
* Afinar diseños responivos o verificar la accesibilidad

---
---
# Instalación


```bash
  # Add Storybook:
  npx storybook init

  # Install
  npm run storybook
  yarn storybook
```

---
---

# Stories

Una `Story` captura el estado del componente en la interfaz de usuario y lo renderiza, escribimos las historias que consideremos interesantes de cada componente.

```js {all|1|5|7-14|16|all}
// Button.stories.js|jsx

import React from 'react';

import { Button } from './Button';

export default {
  /* 👇 The title prop is optional.
  * See https://storybook.js.org/docs/react/configure/overview#configure-story-loading
  * to learn how to generate automatic titles
  */
  title: 'Button',
  component: Button,
};

export const Primary = () => <Button primary>Button</Button>;
```



---
layout: statement
---
<img class=img-ss src="https://storybook.js.org/ff519d6518900d4be0ce86bbf3655913/example-button-args.png" >
