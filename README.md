# Entrevista Angular

![](https://miro.medium.com/max/2800/0*rDChHWWLHxxpXI0a.png)

Bienvenido a tu prueba de __ANGULAR__, a continuación encontrarás una serie de requerimientos con los cuales deberás realizar un ejercicio práctico.

La prueba general se divide en pequeños ejercicios con los cuales se evaluará en práctica:
- Pensamiento lógico
- Resolución de problema
- Tiempo de desarrollo
- Entre otros.


Finalizada la prueba recuerda enviar link del proyecto o tu repositorio a [desarrollo@leangasoftware.es](mailto:desarrollo@leangasoftware.es) con tu información de contacto y en el asunto colocar: ANGULAR-INTERVIEW


> Recomendación: No importa terminar todos los ejercicios, lo más importante es la funcionalidad del ejercicio resuelto(s).

### Antes de empezar:
- Node
- NPM
- [JSON Data](https://jsonplaceholder.typicode.com/)


# Ejercicios

### 1. Vistas.

__HABILIDADES:__
```
ANGULAR
```
__PROBLEMA:__
Se necesitan vistas, y estas deben contener rutas amigables.

__REQUERIMIENTO:__
Se requiere crear un proyecto Angular el cual debe tener como mínimo dos vistas con html básico y sus respectivas rutas.
- Vista principal  __POST LIST__ 
	- RUTA: `/posts` 
	- HTML: Tabla html con 10 registros.
- Vista detalle __POST DETAIL__
	- RUTA: `/post/{id}`
	- HTML: Deberás reflejar en la vista en cualquier parte el `id` pasado por el parámetro. Ejemplo `<p>Este es el post: 12 </p>`  donde "12" es el `id`.
- Vista __404__
	- RUTA: `/404`
	- HTML: A tu gusto.
	- __NOTA:__ Debes poder re-direccionar rutas que no existan a `404`

___
### 2. API.

__HABILIDADES:__
```
ANGULAR
```

__PROBLEMA:__
> La vistas anteriores son representaciones estáticas, ahora vamos a agregarle dinamismo.

__REQUERIMIENTO:__
Se requiere crear un servicio para consumir el siguiente api. [https://jsonplaceholder.typicode.com/](https://jsonplaceholder.typicode.com/)
-	En la vista __POST LIST__ donde anteriormente colocamos un table html estática se debe consumir una lista de post proveniente de `https://jsonplaceholder.typicode.com/posts` y generar el table html dinámico.
-	En la vista __POST DETAIL__ donde anteriormente colocamos un html estático se debe consumir un detalle de post proveniente de `https://jsonplaceholder.typicode.com/posts/{id}`  representar el title y body en la vista.

![](https://i.imgur.com/gaPD2iq.png)

![](https://i.imgur.com/KPe4BUs.png)

___

### 3. COMPONENTE.

__HABILIDADES:__
```
ANGULAR
```

__PROBLEMA:__
> Como todo buen post se necesitan ver los comentarios de dicho post.

__REQUERIMIENTO:__
Se necesita generar un componente el cual se usará en vista del detalle, para cargar una lista de comentarios usando `https://jsonplaceholder.typicode.com/comments?postId={id}` pasando por atributo el id del post. 

Ejemplo `<comentarios post="{id}"/></comentarios>`

![](https://i.imgur.com/8cPCArw.png)

### 4. EMIT

__HABILIDADES:__
```
ANGULAR
```

__PROBLEMA:__
> En ocasiones se necesita emitir información o funciones entre componentes

__REQUERIMIENTO:__
Se requiere emitir la fecha desde el componente `comentarios` con la acción de un botón hacia el componente padre de la vista detalle.

![](https://i.imgur.com/IKDn6vy.png)


### Extra.
Si has llegado hasta este punto, y consideras que tienes tiempo se valora el hecho de que puedas desplegar tu proyecto en [Heroku](https://www.heroku.com/) o en cualquier servidor de tu gusto.

Gracias por participar! 
