![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB | Fundamentos de Vue.js

## Introducción

En este laboratorio, seguirás explorando los fundamentos del uso de Vue.js y sentarás las bases para proyectos más grandes y complicados.

Estas son las cosas que tendrás que lograr durante este laboratorio:

- Crear una estructura de plantilla básica dentro de un nuevo proyecto.
- Mostrar el resultado de una operación JavaScript en el HTML de un componente.
- Mostrar un elemento sólo si una determinada propiedad está establecida como `true`.
- Mostrar una lista de elementos que se almacenan dentro de un componente.
- (Bonus) Cambiar el color de fondo de un elemento al pulsar un botón.

Comencemos.

## Configuración

- Haz un fork de este repo
- Clona este repositorio
- Abra el LAB y comience:

  ```bash
  $ cd lab-vue-basics-es
  $ npm install
  $ npm start
  ```

## La presentación

- Al terminar, ejecuta los siguientes comandos:


  ```bash
  git add .
  git commit -m "done"
  git push origin main
  ```

- Crea un Pull Request para que tus TAs puedan comprobar tu trabajo.

<!-## Getting Started -->

## Instrucciones

### Iteración 1 | Crear una estructura de plantilla básica dentro de un nuevo proyecto

Para este laboratorio, tendrás que crear un nuevo proyecto Vue en una nueva carpeta. Puedes elegir qué opciones quieres incluir, pero recuerda que, de momento, te quedas con Vue 2.

Una de las principales ventajas de Vue (o de cualquier otro framework de frontend) es lo fácil que resulta reutilizar componentes en toda la aplicación. Esto es exactamente lo que vamos a practicar ahora.

Tienes que crear un componente `navbar` y un componente `footer`, que incluirás en todas las páginas interiores de tu aplicación. Sugerencia: si los importas en tu componente App.vue, todas tus páginas internas los mostrarán también.

En este momento, no necesitas preocuparte por el estilo de estos componentes; sólo asegúrate de que están funcionando y eres libre de avanzar a la siguiente tarea.

### Iteración 2 | Mostrar el resultado de una operación Javascript en el HTML de un componente

Ayer practicaste cómo mostrar una `string` dentro de la plantilla de un componente Vue utilizando la sintaxis del bigote`({{}}`). Hoy hemos visto que las cadenas no son lo único que puedes insertar en tu HTML utilizando esta técnica.

Este reto tiene dos partes:

- En primer lugar, sólo tienes que insertar una operación matemática dentro de tu HTML y ver qué pasa. Algo tan simple como `2 + 2` es suficiente aquí.
- Luego, comienza el verdadero reto: tienes que "imprimir" una `string` en tu plantilla, con un giro: esta cadena tiene que ser devuelta por una función. Sugerencia: [este artículo](https://lavalite.org/blog/created-and-mountedin-vuejs) puede arrojar algo de luz sobre cómo se puede hacer esto.

### Iteración 3 | Mostrar un elemento sólo si una propiedad particular es `true`

Una de las principales razones por las que usamos algo como Vue es para poder simplificar las operaciones comunes de JavaScript. Una de las principales ventajas de este framework es que nos permite mostrar elementos condicionalmente de una manera muy sencilla.

¡Vamos a practicar esto! Tu reto aquí es crear un dato booleano dentro de un componente Vue, y vincularlo a un elemento HTML que sólo se mostrará en tu plantilla si la condición es `true`.

Hemos visto las propiedades `v-if` y `v-show` en la clase de hoy; pero si estás atascado, [la documentación oficial](https://v2.vuejs.org/v2/guide/conditional.html) puede ser muy útil aquí.

### Iteración 4 | Mostrar una lista de elementos que están almacenados dentro de un componente

¿Recuerdas lo difíciles que parecían los `for loops` con el JavaScript convencional? Vue hace mucho del trabajo pesado cuando los usamos, y puede permitirnos mostrar una lista de elementos en la pantalla de una manera mucho más fácil.

En este ejercicio, vas a practicar cómo utilizar la directiva `v-for`. El reto tiene los siguientes componentes:

- Tienes que crear una lista de posts dentro de los `datos` de uno de tus componentes Vue. Estos posts necesitan incluir los siguientes datos: título, descripción y contenido; y necesitas al menos tres de ellos.
- Luego, tienes que hacer que los posts "aparezcan" en tu `template` usando la directiva `v-for`.

Una vez más, si estás atascado aquí, [siempre puedes consultar la documentación oficial](https://v2.vuejs.org/v2/guide/list.html).

### Iteración 5 | Bonus | Cambiar el color de fondo de un elemento al pulsar un botón

¿Te apetece un reto más difícil? Vue nos permite hacer cosas bastante "mágicas" de forma simplificada. En este caso, aprenderás a cambiar una propiedad CSS de forma dinámica usando data binding.

No hemos profundizado mucho en este tema; pero aquí hay algunos consejos para apuntar en la dirección correcta:

- Tendrás que crear una clase o una propiedad CSS y [vincularla](https://v1.vuejs.org/guide/syntax.html) a una condición.
- Tendrás que crear un método que cambie la clase o la propiedad y activarlo a través de un clic de botón. Lo practicamos en el laboratorio de ayer, así que no dudes en consultarlo si necesitas ayuda.

¿Te parece bien? Empecemos.

<br/>

¡Feliz codificación! :heart: