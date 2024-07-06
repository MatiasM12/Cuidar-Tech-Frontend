# Cuidar Tech Frontend 💻
Cuidar Tech es un proyecto dedicado a la prevención de la violencia de género mediante el monitoreo de restricciones perimetrales. Este proyecto se basa en la continuación del proyecto original desarrollado por la Universidad Nacional de General Sarmiento (UNGS), que puedes encontrar aquí: https://www.ungs.edu.ar/new/cuidar-tech-una-posible-solucion-tecnologica-para-intervenir-en-casos-de-violencia-domestica-contra-las-mujeres. En esta nueva fase, hemos implementado dos funcionalidades clave: pruebas de vida automáticas y predicción de rutinas para prevenir violaciones de restricciones perimetrales. Ademas de que implementamos otras mejores tanto esteticas como funcionales.

## Funcionalidades Destacadas ⚙️

- Asignar, modificar y monitorear restricciones perimetrales.
- ABM (Alta, Baja y Modificación) de personas, usuarios y juzgados.
- Enviar pruebas de vida a los usuarios, aceptar o rechazar las mismas.
- Generar predicciones de rutina.
- Generar reportes del sistema.
- Configurar parámetros de las rutinas y pruebas de vida.
- Configurar los mensajes que son enviados desde el sistema (WhatsApp, Telegram o correo electrónico).

### Pruebas de Vida Automáticas
Para asegurar la seguridad de los usuarios, implementamos un sistema de pruebas de vida automáticas. Esta funcionalidad permite que las pruebas de vida enviadas a los usuarios sean validadas automáticamente a través de un script de Python que corremos en el servidor.

1. Descripción Técnica
    El script de Python realiza las siguientes tareas:
      - Detecta y reconoce rostros en una imagen proporcionada.
      - Analiza expresiones faciales para determinar si los ojos están abiertos o cerrados, si la boca está abierta o cerrada, y si hay una sonrisa.
      - Utiliza bibliotecas como cv2, face_recognition, y mediapipe para procesar las imágenes y realizar el análisis.

2. Descripción grafica
   
    ![Texto del párrafo (1)](https://github.com/MatiasM12/Cuidar-Tech-Frontend/assets/86579814/2c332b3f-3bb8-4303-b792-e7394c1f3656)
    ![Texto del párrafo (2)](https://github.com/MatiasM12/Cuidar-Tech-Frontend/assets/86579814/35ada39a-9e08-49fd-abed-fab03603725b)
    *(si una de las dos condiciones no se cumple, las pruebas de vida pasan a ser rechazadas)


### Predicción de Rutinas
Utilizando técnicas de Machine Learning, para predecir si el victimario puede violar la restricción perimetral impuesta. Esta funcionalidad es crucial para prevenir posibles incidentes antes de que ocurran, proporcionando una capa adicional de seguridad para las víctimas.

1. Descripción Técnica
      - Se recolectan datos de ubicación y movimientos del victimario.
      - Se entrena el modelo LSTM de Machine Learning para identificar patrones de comportamiento y predecir posibles violaciones de la restricción perimetral.
      - Se calcula la distancia entre las ubicaciones obtenidas por el modelo y las reales, para detectar una posible violación de la perimetral.

2. Descripción grafica

    ![Texto del párrafo (5)](https://github.com/MatiasM12/Cuidar-Tech-Frontend/assets/86579814/d5ee9fbb-9338-44bf-a5c6-114b6eb2e833)

## Cuentas validas 👤
Primero debemos ir a la pagina de ingreso que normalmente seria: http://localhost:4200/ingresar, a menos que tengamos desplegado el sistema.

Las cuentas validas a las que podemos acceder son:

- **Cuenta de supervisor predeterminada:**
  - Correo electrónico: admin@admin.com
  - Contraseña: admin
  - Pantalla de inicio:
    
    ![image](https://github.com/Nicolas2k19/PP2Frontend/assets/86579814/8a1c4123-1317-4e64-9022-89a33a3fc5cb)


- **Cuenta de administrativo:**
  - Correos: gfgrillo3@gmail.com y gustycruz85@gmail.com
  - Para acceder a estas cuentas, sigue el procedimiento de "Olvidaste tu contraseña" y se enviará una nueva contraseña al correo electrónico pp2proyectoviolenciagenero@gmail.com.
    Nota: Si el correo electrónico no funciona o estás en un entorno de desarrollo, podrás ver la nueva contraseña desde la consola del backend.
  - Pantalla de inicio:

    ![image](https://github.com/Nicolas2k19/PP2Frontend/assets/86579814/c14b3015-fea3-48e2-ad76-f09ad988eb30)

    
- **Cuenta de supervisor general:**
  - Correo electrónico: supervisor@general.com
  - Para acceder a estas cuentas, sigue el procedimiento de "Olvidaste tu contraseña" y se enviará una nueva contraseña al correo electrónico pp2proyectoviolenciagenero@gmail.com.
    Nota: Si el correo electrónico no funciona o estás en un entorno de desarrollo, podrás ver la nueva contraseña desde la consola del backend.
  - Pantalla de inicio:
 
    ![image](https://github.com/Nicolas2k19/PP2Frontend/assets/86579814/1b2f423a-419d-4fd4-a17b-417ed2d023bf)


## Instrucciones para ejecutar el código 👨‍🏫

1. **Instalar dependencias:** Ejecuta el siguiente comando para instalar todas las dependencias necesarias:

    ```bash
    npm install --force
    ```

2. **Corregir auditoría de seguridad:** Después de instalar las dependencias, puedes ejecutar el siguiente comando para corregir cualquier problema de seguridad:

    ```bash
    npm audit fix --force
    ```

3. **Ejecutar la aplicación:** Para ejecutar la aplicación, ejecuta el siguiente comando:

    ```bash
    ng serve
    ```

    Esto desplegará la aplicación en el servidor local en [http://localhost:4200/](http://localhost:4200/).

## Configuraciones dentro del código

- **Cambiar la URL del backend:** Si el backend está desplegado en una ubicación diferente, asegúrate de cambiar la URL dentro del archivo `environments/environment.ts`.

    ![image](https://github.com/Nicolas2k19/PP2Frontend/assets/86579814/1e39074e-21d2-4e91-bfc3-1e7443df763f)

## Manual de usuario 📕
Para obtener una guia detallada de como funciona el sistema porfavopr leea el manual de usuario que subimos a esta repositorio.

