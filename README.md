# examenLaravel - Sistema de Inventario

**Estudiante:** Guerrero, Oscar  
**Curso:** Programación Web Básica  
**Periodo:** 2026-10

## Descripción
Sistema de Inventario desarrollado con Laravel. Contiene dos tablas independientes: **Productos** y **Categorías**.

## Requisitos
- PHP >= 8.1
- Composer
- MySQL / XAMPP

## Instalación

```bash
# 1. Clonar el repositorio
git clone https://github.com/oscar3456789/examenLaravel.git
cd examenLaravel

# 2. Instalar dependencias
composer install

# 3. Copiar archivo de entorno
cp .env.example .env

# 4. Generar clave de aplicación
php artisan key:generate

# 5. Configurar base de datos en .env
DB_DATABASE=inventariodb
DB_USERNAME=root
DB_PASSWORD=

# 6. Ejecutar migraciones
php artisan migrate

# 7. Iniciar servidor
php artisan serve
```

## Endpoints de la API

| Método | URL | Descripción |
|--------|-----|-------------|
| GET | /api/productos | Lista todos los productos |
| POST | /api/productos | Crea un nuevo producto |
| GET | /api/categorias | Lista todas las categorías |
| POST | /api/categorias | Crea una nueva categoría |

## Estructura del proyecto

```
app/
  Models/
    Producto.php
    Categoria.php
  Http/Controllers/Api/
    ProductoController.php
    CategoriaController.php
database/
  migrations/
    create_productos_table.php
    create_categorias_table.php
routes/
  api.php
```
