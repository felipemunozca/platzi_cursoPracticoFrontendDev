# Apuntes del curso
A continuación, se describirán algunas características, propiedades, consejos y ayudas entregados por Estefany a la hora de comenzar con el desarrollo FrontEnd de un proyecto.

### Clase 4

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `:root {}` | Es donde se declaran las variables globales a las que se podrán acceder en cualquier momento. Para definir una variable se debe comenzar agregando dos guiones medios -- mas un nombre único (no se pueden colocar nombres con espacios en blanco), un ejemplo de una variable seria: **--white**. Una de las ventajas de utilizar variables es que si se quiere cambiar un valor a futuro, por ejemplo un tamaño o un color, solo se debe hacer una vez y en cada sección donde se use la variable se actualizara automáticamente. Una desventaja o mala practica es colocar un nombre por ejemplo de un color, por ejemplo **--very-light-pink** porque si a futuro se decide cambiar el color como por ejemplo un verde, el nombre de la variable no tendría sentido con el nuevo color, es por eso que es más recomendado nombrar a las variables por lo que van a afectar; un botón, un subtítulo, un background. | 
| `body{ font-family: 'Quicksand', sans-serif; }` | Dentro de la etiqueta body, se agrega la fuente que se eligió en Google Fonts y que se vera en todo el texto que se agregue dentro de la etiqueta < body >. |
| `letter-spacing: 2px; ` | Propiedad para agregar espaciado entre las letras de un botón o de un titulo. |

### Clase 6

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `width: 100%;` | Forma de asignar el 100% del ancho de la pantalla. |
| `height: 100vh;` | Forma de asignar el alto de 100 del viewport height (vh) la pantalla. Con esta propiedad es más fácil manejar los cambios de tamaño de pantalla, por ejemplo: cuando si se gira la pantalla de un teléfono. |
| `display: grid;` | Forma de dividir un contenido en regiones, y luego poder alinearlos en filas y columnas. una forma más fácil de centrar un div, es primero convertirlo a un display grid. |
| `place-items: center;` | Forma de alinear el contenido de una etiqueta que ya cuente con la propiedad grid. Este método es mas fácil y funcional a la hora de centrar el contenido. |
| `grid-template-rows: auto 1fr auto;` | con grid-template-rows le digo que en fila superior, donde está el título y el subtítulo sean de tipo auto, es decir, que tome el tamaño que él quiera. Luego en la sección de los inputs y label sean de 1 fracción. Y finalmente la sección de del botón sea de tipo auto |
| `font-size: var(--lg)` | Esta es la forma de asignar una función declarada en root a una propiedad CSS, se debe usar la palabra var() y entre los paréntesis el nombre de la variable. |
| `display: flex` | Con esta propiedad se puede ubicar un atributo al lado del otro. |
| `border: none` | Forma de quitarle el borde a un contenido, por ejemplo, una tabla, un botón, un menú. |
| `cursor: pointer` | Cuando se pasa el mouse por encima de un botón, por defecto aparece una manito, al utilizar pointer se cambia eso y sigue apareciendo la flecha. |

### Clase 7

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `justify-items: center;` | Se utiliza la propiedad justify-items para centrar los atributos dentro de un div. |
| `justify-content: center;` | La propiedad justify-content se utiliza para definir cómo el navegador distribuye el espacio entre y alrededor de los elementos de contenido a lo largo del eje horizontal. |
| `align-items: center;` | La propiedad align-items se utiliza para establecer el valor de la alineación en todos los hijos directos de una etiqueta. Controla la alineación de los elementos en el eje vertical. |
| `border-radius: 50%;` | Utilizando border-radius al 50% se puede crear un circulo perfecto. |
| `text-decoration: none;` | Propiedad para quitar la línea de subrayado de la etiqueta < a >. |

### Clase 9

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `.input-name, .input-email, .input-password {margin-bottom: 22px;}` | Cuando se debe aplicar el mismo estilo a diferentes clases, en vez de ir agregándole el valor, por ejemplo: 22px a cada clase, se puede escribir cada clase separada por una coma (,) |

### Clase 11

Para reemplazar todos los valores de una etiqueta, por ejemplo la etiqueta < img > todas a la vez, primero se debe presionar las teclas **CTRL + F** y escribir **img**, luego presionar el icono de signo mayor **>** y aparecerá un nuevo recuadro abajo con la opción reemplazar, en donde se debe escribir el nuevo valor que se le quiere asignar a todas las etiquetas < img >

Esta opción también funciona con clases, enlaces y con textos planos que pueda tener el archivo.

### Clase 12

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `grid-template-columns: repeat(auto-fill, 240px);` | La función **repeat** es una propiedad de CSS que permite repetir y definir valores de columnas. Esta función recibirá dos parámetros: la cantidad de columnas que necesito y el tamaño de cada una de las columnas. La propiedad **auto-fill** le dice al navegador, que inserte el numero de columnas o filas que sean necesarios para rellenar un espacio. |
| `place-content: center` | La propiedad place-content permite alinear el contenido a lo largo del bloque y en la dirección inline al mismo tiempo. (Es lo mismo que utilizar las propiedades align-content y justify-content juntas.) |
| `object-fit: cover;` | Esta propiedad hace que la imagen tenga su tamaño original independiente del width y height que se le agregue. |
| `justify-content: space-between;` | Esta propiedad se utiliza para justificar y crear un espacio entre etiquetas. |

### Clase 13

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `.desktop-menu ul li:nth-child(1), .desktop-menu ul li:nth-child(2) {font-weight: bold;}` | Cuando es necesario aplicar estilos a ciertas etiquetas de un listado, en vez de ir creando clases o agregando id, se puede hacer una forma mas profesional, se puede utilizar la pseudo clase **:nth-child()** la cual permite definir los estilos de los hijos de una etiqueta padre. Dentro del paréntesis se establece a a que hijo darle el estilo, por ejemplo, si tengo una lista con 4 elementos, solo aplicare negrita a los hijos 1 y 2.  |
| `display: inline-block;` | **Dato importante:** a los elementos inline no se le puede aplicar un margen directamente, es por este motivo que se debe declarar como un inline de tipo bloque. |

### Clase 14

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `font-weight: 300 !important;` | Debido a la especificidad, como la clase principal ya tiene un estilo, si se requiere cambiar una regla CSS, debo puede utilizar **!important** para que se de prioridad a esta nueva regla. Es importante recalcar que **NO es recomendado** llenar de !important el código. |

### Clase 16

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `grid-template-rows: auto 1fr auto;` | Se utiliza esta propiedad para crear filas en formato grilla con un primer valor automático, un segundo valor de 1 fracción, y un tercer valor también automático. |
| `grid-template-columns: auto 1fr auto auto;` | Se utiliza esta propiedad para crear columnas en formato grilla, mas especifico, en 4 columnas, dentro de las cuales 3 tendrán valores automáticos según el tamaño de la pantalla, y 1 tendrá el valor de 1 fracción. |

### Clase 20

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `position: absolute` | Se utiliza esta propiedad para indicar que la posición que se le dará a una etiqueta sera absoluta y que no puede cambiarse con otra regla. Ademas se puede utilizar para agregar un botón sobre una imagen y en vez de quedar apilados, se sobreponen. |
| `right: 0;` | Propiedad para mover una etiqueta por completo al lado derecho. Se utiliza junto con **position: absolute** para fijar el contenido en el espacio que el diseñador necesite. |
| `z-index: 2;` | La propiedad **z-index** permite cambiar el orden de apilamiento de las etiquetas. Si el valor es positivo, le etiqueta estará arriba, si es negativo, estará por debajo. |
| `object-fit: cover;` | Propiedad CSS para ajustar la imagen y que esta no se vea ni estirada, ni aplastada. |
| `border-radius: 0 0 20px 20px;` | Se puede definir a que esquinas de una etiqueta o imagen se les puede aplicar un border circular. En este caso, se mantendrán iguales las esquinas superiores, mientras se les agrega un diseño circular a las esquinas de abajo de la imagen. |

### Clase 21

| Propiedad CSS | Utilidad |
| ------------- | ------------------------------ |
| `transform: rotate(180deg);` | La propiedad **transform** permite modificar la vista de un elemento. Al utilizarla junto a **rotate**, se puede girar una etiqueta o imagen hacia el lado que indiquen los grados. |