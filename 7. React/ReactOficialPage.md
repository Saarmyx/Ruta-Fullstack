# Aprenderas

- Anidar y crear _componentes_
- Crear marcado y estilos
- Mostrar datos
- Renderizar condiciones y listas
- Responder a los eventos y actualizar la pantalla
- Compartir datos entre _componentes_

# Anidar y crear _componentes_

Las apps de react se componen de _componentes_. Los _componentes_ son partes de la **UI** que tienen logica y aparencia. Un _componente_ puede ser algo tan pequeño como un boton y tan grande como una web

Los _componentes_ son funciones de **JS** que devuelven marcado:

```js
function MyButton() {
  return <button>Soy un boton</button>
}
```

Ahora lo que se declaro en **MyButton**, se puede anidar a otro componente

```js
export default function MyApp() {
  return (
    <div>
      <h1>Bienvendio a mi app</h1>
      <MyButton />
    </div>
  )
}
```

Si nos damos cuenta `<MyButton />` empieza con mayuscula, de esta manera sabremos que es un _componente_ de **React**
