
# TESE-BREAK - Diseño de la base de datos

## Plataforma
Firebase Cloud Firestore.

## 1. Colección: usuarios
Almacena la información de los estudiantes y administradores.

Campos propuestos:
- nombre: String
- correo: String
- rol: String
- activo: Boolean
- fechaRegistro: Timestamp

Identificador: UID de Firebase Authentication.

## 2. Colección: categorias
Clasifica los productos de la cafetería.

Campos:
- nombre: String
- descripcion: String
- activa: Boolean
- orden: Integer

## 3. Colección: productos
Almacena los alimentos y bebidas.

Campos propuestos:
- nombre: String
- descripcion: String
- precio: Number
- categoriaId: String
- disponible: Boolean
- imagenUrl: String

## 4. Colección: pedidos
Registra las compras de los estudiantes.

Campos propuestos:
- usuarioId: String
- productos: Array
- total: Number
- estado: String
- fechaCreacion: Timestamp

## 5. Colección: saldos
Administra el saldo disponible de cada usuario.

Campos propuestos:
- usuarioId: String
- saldoActual: Number
- fechaActualizacion: Timestamp

## 6. Colección: movimientos
Registra las operaciones financieras.

Campos propuestos:
- usuarioId: String
- tipo: String
- monto: Number
- referencia: String
- fecha: Timestamp

## Consideraciones
- Los identificadores de usuario estarán vinculados a Firebase Authentication.
- Los saldos deberán actualizarse mediante operaciones seguras.
- Los pedidos tendrán estados para controlar su preparación.
- Las operaciones financieras deberán conservar un historial.
