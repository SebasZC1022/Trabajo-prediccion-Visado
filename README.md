# Trabajo-prediccion-Visado

# Miembros del Grupo
  - Claudia Yaneth Giraldo Vergara CC CC 1001745178 Ing Industrial
  - Sebastian Zuluaga Cano CC 1020428207 Ing Industrial
  
#Datos

Los datos provienen de https://www.kaggle.com/datasets/jonamjar/h1b-data-set-2017?select=H-1B_Disclosure_Data_FY17.csv y se pueden hacer disponibles ejecutando desde cualquier notebook en Colab los siguientes comandos:

    ! pip install kaggle

    ! mkdir ~/.kaggle

    ! cp kaggle.json ~/.kaggle/

    ! chmod 600 ~/.kaggle/kaggle.json

    ! kaggle datasets download jonamjar/h1b-data-set-2017

    ! unzip h1b-data-set-2017

De esta manera configuramos Kaggle y Kaggle.json antes de descargar y descomprimir el dataset.

Finalmente se ejecutan los siguientes comandos:

    ! import pandas as pd
    ! import numpy as np
    ! nfilas_previas = 20000 #Para realizar una vista previa del dataset vamos a cargar solamente las primeras 20 mil filas, este dato es modificable
    ! data = pd.read_csv('H-1B_Disclosure_Data_FY17.csv', delimiter=',', nrows = nfilas_previas)
