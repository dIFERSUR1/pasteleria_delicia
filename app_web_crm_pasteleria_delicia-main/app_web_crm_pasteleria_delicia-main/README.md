# Pastelería Delicia · CRM web (demo de clase)

Trazabilidad del pedido: el cliente encarga una torta, el empleado avanza su estado y el administrador ve el historial.

| Carpeta | Qué es | Puerto |
|---|---|---|
| `app_web_crm_node_api` | Backend: Node + Express + PostgreSQL (Neon) | 3000 |
| `app_web_crm_react_cliente` | Frontend del cliente (React + Vite) | 5173 |
| `app_web_crm_react_adm_emp` | Frontend de administrador y empleado | 5174 |

## Cómo levantarlo

1. Backend:
   ```bash
   cd app_web_crm_node_api
   npm install
   copy .env.example .env
   npm run db:init
   npm run dev
   ```
   En el `.env` pon TU propia cadena de Neon en `DATABASE_URL`.

2. Cliente (otra terminal):
   ```bash
   cd app_web_crm_react_cliente
   npm install
   npm run dev
   ```

3. Administrador y empleado (otra terminal):
   ```bash
   cd app_web_crm_react_adm_emp
   npm install
   npm run dev
   ```

Usuarios de prueba: `admin@delicia.pe` y `rosa@delicia.pe` (contraseña `123456`).
