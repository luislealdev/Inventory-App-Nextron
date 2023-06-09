## Sobre el proyecto

Se plantea crear un gestor de inventarios y ventas, con un diseño agradable al usuario; donde el mismo pueda agregar nuevos registros sobre ventas y que se descuente del inventario automáticamente.

En el siguiente enlace se encuentrá una fotografía de un ejemplo del diseño que se plantea crear: https://www.pinterest.com/pin/465207836508441514/

Se plantea crear tres apartados principales: Ventas, Inventario, Clientes y Perfil (por el momento). Se accederá a ellos mediante un sidebar como el de la fotografía presentada anteriormente.

##### Ventas

Será la pantalla principal (de inicio). Se presentará la información gráficamente mostrando las ventas totales, ventas netas, productos más vendidos y mejores clientes. Así como un apartado para registrar una nueva venta seleccionando producto(s), cantidad(es) y cliente.

##### Inventario

Se mostrarán productos dados de alta, opciones para modificar, eliminar, agregar y sus cantidades actuales.

##### Clientes

Pantalla muy parecida al inventario, pero con la información de los clientes.

##### Perfil

El usuario podrá cambiar su información personal.

## Tecnologías

Para llevar a cabo esta aplicación de escritorio, se usara Nextron. Nextron es una combinación de Electron (Librería para crear aplicaciones de escritorio con Html, CSS y Js) y Next.js (Framework de react con una forma de manejo de rutas más sencilla).

## Uso

### Descarga el proyecto mediante git clone

### Instala dependencias

```
$ cd my-app

# usando yarn
$ yarn
```

### Usarlo

```
# Modo de desarrollador
$ yarn dev

# Construir para producción
$ yarn build
```

### Docker

Para su uso, se agregó autenticación, para esto en desarrollo vamos a usar docker (Gestor de contenedores), este repositorio ya contiene la configuración para la imagen de docker, solo corre en tu consola antes de hacer el yarn dev:

```
$ docker-compose up -d
```

Con esto la imagen y el contenedor de docker se crearán (asegurate de tener docker desktop corriendo)

### Configuración de variables de entorno

En este repositorio, se ha agregado un template (plantilla) de cómo deberían de verse sus variables de entorno. Lo pueden encontrar en "renderer/.env-template", renombrar este archivo solo por .env y cambiar los valores a sus valores reales.

**No subir su archivo .env al repositorio, es peligroso**

---

Al finalizar de los pasos anteriores, deberás crear una cuenta para estar autenticado, esta cuenta se guardará en tu base de datos local con la imagen de mondodb.
