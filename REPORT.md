## Proyecto: Prueba Módulo 8
## Integrantes:
    Blanca Pinot
    Eduardo Chasco
    Francisco Berroeta
    Francisco Aguilar
Este reporte resume los resultados de las pruebas automáticas ejecutadas, el estado del pipeline de integración continua en Jenkins, y un resumen de los pasos realizados.

## Requerimientos & Desarrollo :books:
1. Gestión del Repositorio Git.

    ● Código del proyecto (subido al repositorio de GitHub).
    
    [Repositorio desafio 8](https://github.com/DL24Modulo8/prueba/tree/dev)
---
2. Configuración básica de la API (2 puntos)

    ● Verificaquela API funciona correctamente utilizando los datos en db.json

    ![Test rut /users ](https://github.com/DL24Modulo8/prueba/blob/dev/documentacion/RutaUsers.png)

    ![Test rut /ueser/:id ](https://github.com/DL24Modulo8/prueba/blob/dev/documentacion/RutaUsersId.png)

---
3. Automatización básica con Jenkins

    :marca_de_verificación_blanca: Estado del Pipeline (Jenkins)
El pipeline configurado en Jenkins incluye las siguientes etapas:
    1. **Checkout del repositorio**
    2. **Instalación de dependencias con `npm install`**
    3. **Ejecución de pruebas con `npm test`**
    4. **Build de imagen Docker**

    :flechas_en_sentido_antihorario: Pasos realizados
    - Crear `index.js` / `app.js`
    - Inicializar proyecto con `npm init -y`
    - Instalar dependencias: `express`, `jest`, `supertest`, `eslint`
    - Crear archivo `Dockerfile`
    - Crear `Jenkinsfile` para automatizar el pipeline
    - Configurar y levantar Jenkins en Docker
    - Conectar Jenkins a GitHub
    - Ejecutar pruebas localmente y validar funcionamiento

    ![Captura Ejecucion Tarea](https://github.com/DL24Modulo8/prueba/blob/dev/documentacion/pipeline.png)

---    
4. Ejecución de pruebas automatizadas

    :advertencia: Problemas encontrados
  - a El pipeline falló inicialmente en la etapa de `npm install`
  - Causa: Jenkins no tenía Node.js configurado en el agente
  - :x: Jenkins usaba `bat` en lugar de `sh` (comando para Windows, no Linux)

    [Captura ERROR ](HTTPS://RUTA_DE_lA_IMAGEN "Captura ERROR ")
---
 5. Reporte y retroalimentación

    - Configura un paso en el pipeline que genere un reporte con los resultados de las
    pruebas.

    ![Captura pipeline generacion reporte](https://github.com/DL24Modulo8/prueba/blob/dev/documentacion/pipelinereport.png)


---
