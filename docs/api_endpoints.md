# Especificación de Consumo de API REST
## Endpoint 1: Autenticación de Usuario
* **Método HTTP:** `POST`
* **Ruta:** `/api/v1/auth/login`
* **Formato de Envío (JSON):**
```json
{
"usuario": "ejemplo@correo.com",
"password": "password123"
}

• Respuesta Exitosa (200 OK):
JSON
{
"status": "success",
"token": "eyJhbGciOiJIUzI1NiIsIn..."
}
Endpoint 2: Consulta de Datos Principales
• Método HTTP: GET
• Ruta: /api/v1/datos
• Descripción: Devuelve el listado de registros mostrados en la pantalla principal de la app
móvil.

---
### PASO 4: MANUAL DE USUARIO MÓVIL (`docs/manual_usuario.md`)
Explica el funcionamiento de la aplicación desde la perspectiva del usuario final:
```markdown
# Manual de Usuario - Aplicación Móvil
## 1. Pantalla de Inicio y Registro
Al abrir la aplicación por primera vez, el usuario visualizará la pantalla de bienvenida. Si no
posee cuenta, debe hacer clic en "Registrarse" e ingresar sus datos básicos.
## 2. Navegación Principal
* **Menú Inferior (Bottom Navigation):** Permite cambiar entre la vista de Inicio, Búsqueda,
Notificaciones y Perfil.
* **Gestión de Datos:** Para actualizar la información de una pantalla, deslizar el dedo hacia
abajo (*Pull to Refresh*).