# Predicción de cobertura de vacunación contra H1N1 y gripe estacionaria
Proyecto para el curso de Inteligencia Artificial para las Ciencias e Ingeniería correspondiente al semestre 2023-2. 

Proyecto realizado por:

Manuela Ospina Giraldo - C.C. 1007232820 - Bioingeniería

Marisol Correa Gutierrez - C.C. 1007223653 - Bioingeniería

Eliana Salas Villa - C.C. 1193579584 - Bioingeniería

Para agregar un conjunto de datos de Kaggle a Google Colab utilizando un archivo JSON de token de Kaggle, sigue estos pasos:

1. *Preparar tu token de Kaggle*:

   - Ve a tu perfil en Kaggle (https://www.kaggle.com/account).
   - En la sección "API", haz clic en "Create New API Token". Esto descargará un archivo JSON llamado `kaggle.json` a tu computadora. Este archivo contiene tus credenciales de Kaggle.

2. *Subir el archivo JSON a Google Colab*:

   - Abre Google Colab (https://colab.research.google.com/).
   - En Colab, haz clic en el ícono de carpeta en el panel izquierdo para abrir la sección de archivos.
   - Haz clic en el ícono de "Subir" y selecciona el archivo `kaggle.json` que descargaste previamente. Esto subirá el archivo a tu entorno de Colab.

3. *Instalar la biblioteca de Kaggle*:

   - Ejecuta el siguiente comando en una celda de Colab para instalar la biblioteca de Kaggle:

     python
     !pip install kaggle
     

4. *Mover el archivo JSON a la ubicación correcta*:

   - A continuación, debes mover el archivo `kaggle.json` al directorio correcto donde la biblioteca de Kaggle espera encontrarlo. Utiliza el siguiente comando para hacerlo:

     python
     !mkdir -p ~/.kaggle
     !mv kaggle.json ~/.kaggle/
     

5. *Cambiar los permisos del archivo JSON*:

   - Para proteger tus credenciales, debes asegurarte de que el archivo JSON tenga permisos adecuados. Utiliza el siguiente comando para establecer permisos restrictivos:

     python
     !chmod 600 ~/.kaggle/kaggle.json
     

6. *Descargar el conjunto de datos de Kaggle*:

   - Ahora puedes usar la biblioteca de Kaggle para descargar el conjunto de datos que deseas en Colab. Usa el siguiente comando como ejemplo (reemplaza `<nombre-del-conjunto-de-datos>` con el nombre del conjunto de datos que deseas):

     python
     !kaggle datasets download -d <nombre-del-conjunto-de-datos>
     

   - Esto descargará el conjunto de datos en formato ZIP a tu entorno de Colab.

7. *Descomprimir el conjunto de datos*:

   - Descomprime el archivo ZIP descargado usando el siguiente comando (reemplaza `<nombre-del-archivo.zip>` con el nombre del archivo que descargaste):

     python
     !unzip <nombre-del-archivo.zip>
     

   - Esto descomprimirá el conjunto de datos y podrás acceder a sus archivos para su análisis.

Con estos pasos, habrás agregado un conjunto de datos de Kaggle a tu entorno de Google Colab utilizando tu archivo JSON de token de Kaggle. Ahora puedes comenzar a trabajar con los datos en tu notebook de Colab.
