## ¿Qué es Snyk?
- Snyk es una herramienta de seguridad para desarrolladores que detecta y soluciona vulnerabilidades en dependencias de proyectos (como npm en nuestro caso), así como problemas en el código, contenedores y configuraciones de infraestructura como código.
- Su principal objetivo es ayudarte a mantener tu aplicación segura desde la etapa de desarrollo

## ¿Que hace exactamente Snyk?
- Analiza tu proyecto para encontrar vulnerabilidades conocidas en las bibliotecas que usas
- Sugiere soluciones automáticas, como actualizar a versiones seguras
- Se integra fácilmente con GitHub, GitLab, VSCode, etc.
- Monitorea continuamente tu repositorio si lo conectas, notificándote cuando aparezcan nuevas amenazas

## Ejemplo práctico realizado por nosotros
- Al ejecutar `snyk test`, Snyk escaneó el `package.json` y `package-lock.json` para detectar vulnerabilidades conocidas en las versiones de las dependencias
- Encotró **17 issues** y **102 vulnerabilidades**, dónde vimos que habían algunas relacionadas a dependencias desactualizadas
- Al correr `npm install axios@^1.8.3` actualizamos `axios` a una versión más reciente que corrige algunos de esos problemas
- Al volver a escanear con `snyk test`, el número bajó a **15 issues** y **100 vulnerabilidades**, lo cual indica que **2 issues** fueron resueltos solo por actualizar una dependencia.