# 🔐 Auth Service

**Puerto:** `8081`
**Base de Datos:** `db_auth`

Microservicio encargado de la seguridad, registro de usuarios y generación de **Tokens JWT**.

## ⚠️ Nota Importante para Pruebas de Integración
El sistema asume una sincronización secuencial de IDs:
1.  Al crear un usuario aquí, note el ID asignado (ej. **ID: 1**).
2.  Este ID será necesario para crear el perfil correspondiente en **Customer Service**.

## 🛠️ Base de Datos
```sql
CREATE DATABASE db_auth; -- Para usuarios y roles
```

---
### 🔗 Mapa de Arquitectura
0. [Config data](https://github.com/AlexaRamirezV/config-data.git)
1. [Config Server](https://github.com/AlexaRamirezV/config-service.git)
2.  [Registry Service (Eureka)](https://github.com/AlexaRamirezV/registry-service.git)
3.  [Gateway Service](https://github.com/AlexaRamirezV/gateway-service.git)
4.  [Admin Service](https://github.com/AlexaRamirezV/admin-service.git)
5.  APIs del sistema:
   * ➡️ **[Auth]**
   * [Customer](https://github.com/AlexaRamirezV/DWB-customer.git)
   * [Product](https://github.com/xEriis/Backend.git)
   * [Invoice](https://github.com/AlexaRamirezV/DWB-invoice.git)
