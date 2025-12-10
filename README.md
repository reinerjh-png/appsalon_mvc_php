# App Salon - PHP MVC & SASS

## 1. Requisitos Previos
- **PHP** (versión 8.0 o superior recomedada)
- **Composer** (para dependencias de PHP)
- **Node.js & NPM** (para dependencias de desarrollo y SASS)
- **MySQL** (Base de datos)

## 2. Instalación

### Dependencias de PHP
Este paso es crítico. Si no tienes `composer` instalado globalmente, descomprime el ejecutable en la raíz o instálalo.
```bash
composer update
```
*Esto creará la carpeta `vendor`.*

### Dependencias de JavaScript/SASS
```bash
npm install
```
*Esto creará la carpeta `node_modules`.*

## 3. Configuración de Base de Datos

1.  Asegúrate de tener un servidor MySQL corriendo.
2.  Importa el archivo SQL para crear la estructura de la base de datos:
    - Archivo: `appsalon_mvc_php.sql` (en la raíz del proyecto)
    - Puedes usar PHPMyAdmin o Workbench.
3.  Revisa el archivo `.env` en la raíz del proyecto y ajusta tus credenciales si son diferentes:
    ```env
    DB_HOST=localhost
    DB_USER=root
    DB_PASS=      <-- Pon tu contraseña aquí si tienes
    DB_NAME=appsalon_mvc_php
    ```

## 4. Ejecución

### Compilar Estilos (SASS) y JS
Para compilar los archivos y observar cambios:
```bash
npm run dev
```

### Iniciar Servidor PHP
Puedes usar el servidor integrado de PHP. Ejecuta este comando desde la raíz del proyecto:
```bash
php -S localhost:3000 -t public
```

Ahora abre tu navegador en: [http://localhost:3000](http://localhost:3000)
