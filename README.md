# Creador De Backends con EF

Este proyecto proporciona un archivo .bat ejecutable para poder crear backends en cuestion de minutos con 4 capas en c#.

## Detalles Faltantes 
en 2 archivos faltan poner una informacion que no he logrado corregir entonces solo ingresar esas 2 lineas: 

en Params de la carpeta Helpers en la linea 23 "set => _search = ( "";" deber de ser "set => _search = (!string.IsNullOrEmpty(value))? value.ToLower(): "";"

en el UserService en la linea en la linea 114 "if (rolExists = null)" deberia de ser if "(rolExists != null)"
## Características 🌟

- creacion de entidades, interfaces, repositorios, dtos, controllers, unidad de trabajo, apiContext
- rapidez a la hora de crear backends pequeños siendo estos creados facilmente
  
y dentro del backend viene:
- Registro de usuarios.
- Autenticación con usuario y contraseña.
- Generación y utilización del token.
- CRUD completo para cada entidad.
- Vista de las consultas requeridas.
- Para cada controlador GET una version con paginacion y otra sin paginacion.

## Uso 🕹

Una vez que descargue el archivo solo tendra que ejecutarlo y el se encargara de todo el apartado de crear carpetas, descargar dependencias
una vez cree todo ese apartado le preguntara el numero de entidades que requiere para despues preguntar el nombre de cada entidad, una vez echo eso
el archivo se encargara del resto

## Desarrollo de los Endpoints requeridos⌨️

Cada Endpoint tiene su versión 1.0 y 1.1, al igual que están con y sin paginación.

Para consultar la versión 1.0 de todos se ingresa únicamente el Endpoint; para consultar la versión 1.1 se deben seguir los siguientes pasos: 

En el Thunder Client se va al apartado de "Headers" y se ingresa lo siguiente:

![image](https://github.com/SilviaJaimes/Proyecto-Veterinaria/assets/132016483/8044ee3d-76d9-4437-9f08-da8e5d7cff9a)

Para realizar la paginación se va al apartado de "Query" y se ingresa lo siguiente:

![image](https://github.com/SilviaJaimes/Proyecto-Veterinaria/assets/132016483/22683e46-037e-4f30-96b8-161df8622b40)

## Desarrollo ⌨️
Este proyecto utiliza varias tecnologías y patrones, incluidos:

Entity Framework Core para la ORM.
Patrón Repository y Unit of Work para la gestión de datos.
AutoMapper para el mapeo entre entidades y DTOs.
.bat para la creacion del ejecutable 

## Agradecimientos 🎁

A todas las librerías y herramientas utilizadas en este proyecto.

A ti, por considerar el uso de este sistema.

por Owen 🦝
![image](https://github.com/omapache/Veterinaria/assets/133465475/8ff4353b-89ed-4efa-9ae6-0b56f165343e)
