# INSTRUCCIONES DE INSTALACION Y PASOS PARA LEVANTAR EL BAKCEND.

## Herramientas Necesarias:

- ### XAMPP - (Tener Configurado Apache y MySQL)
- ### Gestor de DB MySQL (Recomendamos Workbench, aunque tambien funciona con phpMyAdmin)
- ### Visual Studio Code 
- ### Node js (16.14.0 o superior). (Testeado en 16.14.2)


## Instrucciones de Instalacion:

1. Descargar o Clonar el Repositorio

2. En Visual Studio Code, con el proyecto abierto, dirigirse a la carpeta del Backend. 

3. Lanzar una terminal e instalar las dependencias con el siguiente comando: 
>- `npm install` 

3. Abrir XAMPP y activar los Modulos de Apache y MySQL. (Ambos deben aparecer en color verde, lo cual indica su correcta activacion).

>- Nota: En caso de tener configurado un puerto MySQL con algun gestor no es necesario activar el Modulo MySQL en XAMPP. 

4. Crear una base de Datos en el gestor de MySQL que se este utilizando. (Reiteramos, recomendamos Workbench en su version 8.0).
>- crearla con el nombre `chatbot_tp2`

5. En el proyecto, dirigirse a la carpeta config y en el archivo `config.json` configurar la seccion `development` con sus propios datos. 

```
"development": {
    "username": "su_usuario",
    "password": "su_password",
    "database": "chatbot_tp2",
    "host": "localhost", (En caso de error, intentar con 127.0.0.1)
    "dialect": "mysql"
  },
```
5. En Visual Studio Code, con el proyecto abierto, lanzar una terminal y ejecutar el siguiente comando: 
>- `npm run devstart` 

```
Si todos los pasos se realizaron correctamente. En su terminal deberia ver un mensaje como: 

`Servidor corriendo en puerto 4000` 

```


