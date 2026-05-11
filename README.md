# Análisis de la evolución del precio del petróleo y eventos geopolíticos

Proyecto de análisis de datos en Python sobre la evolución histórica del precio del petróleo Brent, incorporando visualizaciones, métricas anuales y contexto geopolítico para interpretar posibles cambios en la tendencia del mercado energético.

## Objetivo del proyecto

El objetivo de este proyecto es realizar un análisis exploratorio sencillo del precio histórico del petróleo Brent, aplicando un flujo básico de análisis de datos:

- carga de datos;
- limpieza y transformación;
- análisis temporal;
- visualización de resultados;
- análisis de eventos relevantes;
- exportación de resultados para Power BI.

## Herramientas utilizadas

- Python
- pandas
- matplotlib
- Jupyter Notebook
- Power BI
- DAX

## Fuente de datos

Los datos del precio del petróleo Brent se han descargado desde FRED, utilizando la serie histórica diaria del Brent.

El dataset contiene precios diarios del Brent expresados en dólares por barril.

## Proceso realizado

El análisis se ha estructurado en los siguientes pasos:

1. Carga del dataset original.
2. Revisión inicial de la estructura del DataFrame.
3. Renombrado de columnas.
4. Conversión de fechas a formato datetime.
5. Conversión del precio Brent a formato numérico.
6. Eliminación de valores nulos.
7. Creación de variables temporales: año, mes y año-mes.
8. Análisis de la evolución histórica del precio.
9. Cálculo del precio medio anual.
10. Cálculo del precio máximo y mínimo por año.
11. Cálculo de la variación anual porcentual.
12. Visualización de eventos económicos y geopolíticos relevantes.
13. Análisis del precio medio antes y después de eventos concretos.
14. Exportación de resultados en CSV para su posterior análisis en Power BI.

## Análisis de eventos

Se ha creado una función en Python para comparar el precio medio del Brent antes y después de determinados eventos relevantes.

La función calcula:

- precio medio antes del evento;
- precio medio después del evento;
- variación porcentual entre ambos periodos.

Algunos de los eventos incluidos son:

- Invasión de Kuwait por Irak
- Guerra del Golfo
- Crisis financiera asiática
- Atentados del 11-S
- Invasión de Irak
- Huracán Katrina
- Crisis financiera global de 2008
- Primavera Árabe
- Acuerdos de la OPEP
- COVID-19
- Invasión rusa de Ucrania
- Guerra Israel-Hamás
- Ataques en el Mar Rojo

El análisis no busca demostrar una relación causal directa entre los eventos y la evolución del precio, sino contextualizar los movimientos del mercado alrededor de fechas relevantes.

## Archivos generados

El proyecto genera los siguientes archivos:

- `brent_limpio.csv`: dataset limpio con las variables temporales añadidas.
- `analisis_eventos_brent.csv`: tabla con el análisis antes y después de cada evento.
- `precio_brent_eventos.png`: gráfico con la evolución del Brent y eventos destacados.

## Preparación para Power BI

Los archivos CSV exportados están preparados para ser cargados en Power BI.

A partir de ellos se pueden crear medidas DAX como:

- precio medio Brent;
- precio máximo Brent;
- precio mínimo Brent;
- variación anual;
- media móvil;
- volatilidad;
- comparación entre periodos.

Esto permite ampliar el proyecto con un dashboard interactivo.

## Conclusiones

El análisis muestra que el precio del petróleo Brent presenta una elevada volatilidad a lo largo del tiempo. Los datos permiten identificar periodos de fuertes subidas y bajadas, especialmente en contextos de crisis económicas, tensiones geopolíticas o cambios relevantes en la oferta y la demanda energética.

Este proyecto demuestra un flujo completo de análisis de datos: carga, limpieza, transformación, visualización, creación de funciones y exportación de resultados para herramientas de visualización como Power BI.

