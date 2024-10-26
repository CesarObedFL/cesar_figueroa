# _Prueba Burden_

Esta app es para la acreditación de la prueba

# Tecnologías

<p align="center">
    <a href="https://laravel.com/" target="_blank" rel="noreferrer"> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/laravel/laravel-original.svg" alt="laravel" width="40" height="40"/> </a>
    <a href="https://vuejs.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original-wordmark.svg" alt="vuejs" width="40" height="40"/> </a> 
    <a href="https://axios-http.com/docs/intro" target="_blank" rel="noreferrer"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/axios/axios-plain-wordmark.svg" alt="axios" width="40" height="40"/> </a> 
    <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a>
    <a href="https://mariadb.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/mariadb/mariadb-icon.svg" alt="mariadb" width="40" height="40"/> </a> 
</p>

- [Laravel] - Laravel 11 como tecnología principal Backend
- [Vue3] - Vue 3 Composition API como tecnología principal Frontend
- [Bootstrap] - Como framework de diseño responsivo css
- [Axios] - Como tecnología principal para la comunicación asincrona y hacer peticiones entre en frontend y el backend
- [MariaDB] - Como base de datos relacional


# Instalación y Requerimientos

## _requerimientos_

- php ^8.1
- composer ^2.2.4 
- gd php library

## _instalación_

- create the database: burden_db
    from command line: `CREATE DATABASE burden_db;`
- create the database user: burden_db_user
    from command line: `CREATE USER 'burden_db_user'@'localhost' IDENTIFIED BY 'secret';`
- give permission to the user created:
    from command line: `GRANT PRIVILEGE ON burden_db.* TO 'burden_db_user'@'localhost';`

```
1. Clona este repositorio con el comando `git clone repo_url`
2. Corre el comando `composer install`
3. Copia el archivo `.env.example` a `.env` 
4. Actualiza las variables de configuración como la base de datos:
    - DB_CONNECTION=mysql
    - DB_HOST=127.0.0.1
    - DB_PORT=3306
    - DB_DATABASE=burden_db
    - DB_USERNAME=burden_db_user
    - DB_PASSWORD=secret
5. Corre `php artisan key:generate` para generar la app key
6. Corre `php artisan migrate --seed` para generar las migraciones y datos de prueba
```

## _login_

para ingresar al sistema despues de hacer las migraciones usa las siguientes credenciales:

- user: test1@example.com
- pass: secret

o puedes crear un nuevo usuario en la ruta: `/register`

[Laravel]: <https://laravel.com/docs/8.x>
[Bootstrap]: <https://getbootstrap.com/docs/5.0/getting-started/introduction/>
[Vue3]: <https://vuejs.org/>
[Axios]: <https://axios-http.com/docs/intro>
[MariaDB]: <https://mariadb.com/kb/en/documentation/>