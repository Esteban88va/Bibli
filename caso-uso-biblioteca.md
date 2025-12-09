# 📘 Caso de Uso: Préstamo de Libros — Biblioteca

## 🎭 Actores
- Usuario
- Bibliotecario
- Administrador

## 🧩 Casos de Uso Principales
```plaintext
Solicitar préstamo
 ├── <<include>> Ver disponibilidad
 ├── <<include>> Validar usuario
 ├── <<extend>> Reservar libro (si no disponible)
 ├── <<include>> Registrar préstamo
 └── <<extend>> Generar comprobante

Devolver libro
 ├── <<include>> Registrar devolución
 └── <<extend>> Registrar multa (si hay retraso)

Consultar historial de préstamos
 └── <<include>> Filtrar por usuario

Auditar movimientos
 └── <<include>> Exportar registros
