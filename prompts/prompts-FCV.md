# Prompts

## Prompt 1 - Claude 3.7

Asume el rol de un experto DevOps.
Tengo un proyecto backend y necesito configurar una pipeline en GitHub Actions que, tras el trigger "push a una rama con un Pull Request abierto", siga los siguientes pasos:
* Pase unos tests de backend.
* Genere un build del backend.
* Despliegue el backend en un EC2. 

Tu goal es generar un prompt destinado a Cursor, por lo que necesito que sea lo más claro y conciso posible, como si estuviera destinado a un desarrollador junior sin experiencia. Es importante que no des detalles técnicos específicos solo instrucciones. El output debe ser en md.


## Prompt 2 - Cursor agent + Claude 3.7 thinking

# Prompt para Cursor: Configuración de Pipeline en GitHub Actions

Necesito crear un archivo de configuración para GitHub Actions que automatice el proceso de integración continua y despliegue de mi aplicación backend. El workflow debe:

1. Activarse cuando se realice un push a una rama que tenga un Pull Request abierto
2. Ejecutar tests de backend
3. Generar un build del proyecto
4. Desplegar la aplicación en una instancia EC2 de AWS

Por favor, genera un archivo YAML para GitHub Actions (.github/workflows/backend-ci-cd.yml) con estos requisitos. Incluye comentarios explicativos que me ayuden a entender cada sección. No tengo experiencia previa con GitHub Actions o despliegues automatizados.

Necesito:
- La estructura básica del archivo YAML
- Cómo configurar el trigger correcto
- Cómo separar el proceso en jobs para testing, building y deployment
- Cómo gestionar las credenciales de AWS de forma segura
- Pasos claros para el despliegue en EC2

Explícame también dónde debo almacenar mis secretos en GitHub para que el workflow funcione correctamente.

## Prompt 3 - Cursor agent + Claude 3.7 thinking

Necesito que el despliegue sea en pull request abiertas contra main