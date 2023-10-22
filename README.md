# Predicción de cobertura de vacunación contra H1N1 y gripe estacionaria
Proyecto para el curso de Inteligencia Artificial para las Ciencias e Ingeniería correspondiente al semestre 2023-2. 

Proyecto realizado por:

Manuela Ospina Giraldo - C.C. 1007232820 - Bioingeniería

Marisol Correa Gutierrez - C.C. 1007223653 - Bioingeniería

Eliana Salas Villa - C.C. 1193579584 - Bioingeniería

Competencia: H1N1 and Seasonal Flu Vaccines - Aprendizaje para predecir un problema multi-etiqueta con las vacunas contra la gripe H1N1 y estacional

Para agregar un conjunto de datos de Kaggle a Google Colab utilizando un archivo JSON de token de Kaggle, siguiendo estos pasos:

*1. Preparar el token de Kaggle:*
   - Ir al perfil en Kaggle (https://www.kaggle.com/account).
   - En la sección "API", hacer clic en "Create New API Token". Esto descargará un archivo JSON llamado kaggle.json a tu computadora. Este archivo contiene tus credenciales de Kaggle.

*2. Subir el archivo JSON a Google Colab:*

   - Abrir Google Colab (https://colab.research.google.com/).
   - En Colab, hacer clic en el ícono de carpeta en el panel izquierdo para abrir la sección de archivos.
   - Hacer clic en el ícono de "Subir" y selecciona el archivo kaggle.json descargado previamente. Esto subirá el archivo al entorno de Colab.

*3. Instalar la biblioteca de Kaggle:*

   - Ejecutar el siguiente comando en una celda de Colab para instalar la biblioteca de Kaggle:

     ```!pip install kaggle```

*4. Mover el archivo JSON a la ubicación correcta:*

   - Mover el archivo kaggle.json al directorio correcto donde la biblioteca de Kaggle espera encontrarlo. Utilizar el siguiente comando:

     ```!mkdir -p ~/.kaggle```
     ```!mv kaggle.json ~/.kaggle/```
     
*5. Cambiar los permisos del archivo JSON:*

   Para proteger tus credenciales, se debe asegurar que el archivo JSON tenga permisos adecuados. Para ello, se utiliza el siguiente comando para establecer permisos restrictivos:

     ```!chmod 600 ~/.kaggle/kaggle.json```

*6. Descargue el conjunto de datos de Kaggle:*

   - Usar la biblioteca de Kaggle para descargar el conjunto de datos que deseas en Colab. 

     ```!kaggle datasets download -d <H1N1_Flu_Vaccines>```

   - Esto descarga el conjunto de datos en formato ZIP a el entorno de Colab.

*7. Descomprimir el conjunto de datos:*

   - Descomprima el archivo ZIP descargado usando el siguiente comando :

     ! unzip <H1N1_Flu_Vaccines.zip>
     
   - Esto descomprime el conjunto de datos y se puede acceder a los archivos para su análisis.
