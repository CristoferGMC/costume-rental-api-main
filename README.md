
# Costume Rental API

API RESTful desarrollada en Laravel para la gestión de alquiler de disfraces, piezas y categorías. Esta API es un complemento extra para proyectos de alquiler de disfraces.

## Requisitos

- **PHP** >= 8.2
- **MySQL**
- **Composer**
- **Node.js y npm** (opcional para assets)
- **Extensiones:** Laravel Sanctum, JWT Auth

## Instalación

1. Clona el repositorio y entra a la carpeta del proyecto.
2. Instala dependencias backend:
	```
	composer install
	```
3. Copia el archivo `.env.example` a `.env` y configura tu base de datos y llaves JWT.
4. Ejecuta las migraciones y seeders:
	```
	php artisan migrate --seed
	```
5. Genera la clave JWT:
	```
	php artisan jwt:secret
	```
6. Inicia el servidor:
	```
	php artisan serve
	```

## Endpoints principales

- **Autenticación:**
  - `POST /api/auth/register` — Registro de usuario
  - `POST /api/auth/login` — Login y obtención de token JWT
  - `POST /api/auth/logout` — Cierre de sesión
  - `POST /api/auth/refresh` — Refrescar token
  - `POST /api/auth/me` — Información del usuario autenticado

- **Recursos principales:**
  - `GET /api/categories` — Listado de categorías
  - `GET /api/costumes` — Listado de disfraces
  - `GET /api/pieces` — Listado de piezas
  - `GET /api/rentals` — Listado de alquileres
  - `GET /api/return-records` — Listado de devoluciones

  *(Incluye endpoints para crear, actualizar, mostrar y eliminar cada recurso)*

## Seguridad

- Autenticación basada en JWT.
- Rutas protegidas para operaciones de escritura.

## Testing

- Incluye pruebas con PestPHP.
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Redberry](https://redberry.international/laravel-development/)**
- **[Active Logic](https://activelogic.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
