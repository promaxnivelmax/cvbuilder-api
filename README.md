# CV Builder API – GA7-220501096-AA5-EV03
Servicios web del proyecto formativo **CV Builder** (hoja de vida en línea) · Iván Gerardo Rodríguez Bustamante · ADSO 3186596 · SENA Barrancabermeja.

## Ejecutar
```bash
npm install
npm start          # http://localhost:4000
npm test           # pruebas con Newman (colección de Postman)
```
Documentación interactiva (Swagger / OpenAPI 3): http://localhost:4000/api/docs

## Módulos
| Archivo | Responsabilidad |
|---|---|
| src/server.js | Servidor Express, rutas de perfil, hoja de vida y cuenta |
| src/auth.js | Registro, inicio de sesión y token JWT |
| src/crud.js | Servicios CRUD genéricos (formación, experiencia, habilidades, referencias) |
| src/db.js | Base de datos SQLite y creación de tablas |
| docs/openapi.json | Documentación de cada servicio |
| postman/ | Colección de pruebas y reporte |

## Servicios (23)
Salud · Autenticación (registro, login) · Perfil (consultar, guardar) · Hoja de vida completa · Eliminar cuenta · CRUD de formación, experiencia, habilidades y referencias.
Todas las rutas, excepto salud y autenticación, exigen el encabezado `Authorization: Bearer <token>`.
