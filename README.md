# Coder-DE

Data Engineering Flex

Repositorio actividades curso Data Engineering Flex

Importante: para ejecutar el proyecto se debe crear un archivo .env en la carpeta raiz del mismo. Y acceder con sus propias credenciales a la base de datos.





Entregable 1

Objetivos generales
Generar un script (formato .py o .ipynb) que funcione como prototipo (MVP) de un ETL para el proyecto final
El script debería extraer datos desde una API en formato JSON para ser manipulado como diccionario utilizando el lenguaje Python
Generar una tabla para ser almacenada en una base de datos a partir de información una API.





#Actividades

#Se genero el script: Primer pre entrega.py 




import finnhub
import requests
import pandas as pd
import psycopg2

conexion API
finnhub_client = finnhub.Client(api_key="YOUR_API")

datos API
lista = finnhub_client.company_earnings('NVDA', limit=5)
for e in lista:
    for x, y in e.items():
        print(x, y)










#Se creo la tabla en Redshift







![redshift primer entrega](https://github.com/user-attachments/assets/19dde5f9-cd37-4e17-8067-34a10c3589b0)


















