# 202402_INFO282_portalrobleaustral
Plataforma web Roble Austral para el curso INFO282 

## Mejora documentacion de requisitos 
1. Diferenciar requerimientos y especificaciones
        
        Requerimientos 
        - Se requiere enrutamiento para navegación entre vistas.
        - El backend debe gestionar usuarios administradores.
        - El backend debe conectarse a una base de datos MongoDB.
        - El backend debe exponer una API RESTful.
        
        Especificaciones 
        - Uso de `react-router-dom` para manejar rutas.
        - Uso de `react-icons` y `@fortawesome/react-fontawesome` para incorporar íconos SVG.
        - Uso de `Poetry` como gestor de dependencias de Python.
        - Uso de `uvicorn` para levantar el servidor ASGI.

2. Requisitos funcionales y no funcionales
        
        Requisitos funcionales
        - La aplicación debe consumir una API externa en `http://localhost:4008`.
        - El backend debe permitir iniciar sesión como administrador mediante credenciales definidas en el archivo `.env`.
        - El backend debe responder a solicitudes HTTP en el puerto 4008.
        
        Requisitos no funcionales
        - El backend debe permitir la escalabilidad
        - El backend debe ser seguro 

3. ¿Existe algún modelo arquitectónico?

        Hay una arquitectura cliente-servidor con separación clara entre frontend y backend:
        
        - El frontend actúa como cliente React, que consume servicios de una API.
        - El backend actúa como servidor API REST usando FastAPI y gestiona la lógica de negocio y la base de datos MongoDB.
        
        Podría documentarse como una arquitectura de tres capas:
        - Presentación (React),
        - Lógica de negocio (FastAPI),
        - Persistencia (MongoDB).

## Casos de prueba INFO-290
- https://docs.google.com/spreadsheets/d/1jEr677iI3VnfXAMs2sS9h2A_DuqMxdQNU3vupyiIqp8/edit?hl=es&gid=0#gid=0

