En react ya viene preparado el json, para hacer testing con react testing library

Esta libreria se construye sobre dom teesting lybrari, es un conjunto de utilidades que nos facilita hacer el testing en react

Para jsx

```bash
npm install --save-dev @testing-library/react @testing-library/dom
```

Para tsx

```bashnpm install --save-dev @testing-library/react @testing-library/dom @types/react @types/react-dom

```

Debemmos hacerlo ya que el front no es el mismo de hace mucho tiempo, y la idea es automatizar muchas ccosas en este caso

Podeemos hacer nombreDelArchivoQueSeHaraText.test.js o en una carpeta llamada Test

primero importamos las librerias (obviamente)

```jsx
import React from 'react'
import '@testing-library/jest-dom/extend-expect'
import { render } from '@testing-library/react'
// Depues el componete que vamos a testear
import Note from './Note'

test ('renders content', () => {
    const note = {
        content: 'This is a test',
        important: true
    }
const component = render(<Note note={note}/>)

console.log(componet)

// De esta manera renderizamos nuestro componente y nos permmite ver todo nuestro componente
}
podemos hacer un getBy para buscara propiedad

// Aqui vera si
component.getByText('Camion')

```
