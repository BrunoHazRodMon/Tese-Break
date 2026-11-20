
# TESE-BREAK - Base de datos

## Tecnologia
Firebase Cloud Firestore.

## Identificacion
- Proyecto: TESE-BREAK
- Project ID: tese-break-22cbd
- Base de datos: (default)

## Estructura de colecciones

### categorias
Almacena las categorías de alimentos y bebidas.

Campos:
- nombre: String
- descripcion: String
- activa: Boolean
- orden: Integer

### productos
Almacena los alimentos y bebidas disponibles.

### usuarios
Almacena los perfiles de estudiantes y administradores.

### saldos
Registra el saldo disponible de los usuarios.

### movimientos
Registra recargas, compras y devoluciones.

### pedidos
Almacena los pedidos realizados por los estudiantes.

## Archivos de respaldo

- backups/firestore-backup.json
- config/firestore.rules
- config/firestore.indexes.json

## Seguridad
Las reglas iniciales bloquean el acceso hasta configurar
la autenticación y los permisos correspondientes.

## Recuperacion
Se implementará un procedimiento de exportación y
restauración de los datos de Cloud Firestore.

## Importante
No almacenar contraseñas, claves privadas ni información
personal real en respaldos de repositorios públicos.
