• Este proyecto analiza un conjunto de datos de ventas de videojuegos, explorando las tendencias del mercado, la popularidad de las plataformas, el rendimiento de los géneros y el comportamiento del consumidor regional entre 2010 y 2016. El objetivo es obtener insights utiles y proporcionar recomendaciones basadas en datos para una tienda minorista de videojuegos online , "Ice", con el fin de optimizar su estrategia para 2017 y años siguientes.

## El problema
La tienda online Ice necesita entender qué factores impulsan las ventas de videojuegos (plataforma, género, puntuaciones, región) para optimizar inventario, campañas y estrategia comercial en 2017 y años siguientes. El objetivo es identificar tendencias, plataformas y géneros prioritarios, además de medir el impacto de las reseñas en ventas por región.

## Datos

Archivo principal: games.csv (DataFrame con columnas típicas: name, platform, year_of_release, genre, na_sales, eu_sales, jp_sales, other_sales, critic_score, user_score, rating).

Periodo de interés: 2010–2016 (se selecciona por estabilidad de plataformas relevantes en ese intervalo).

Limpiezas realizadas: manejo de NaN en name/genre/year_of_release, conversión de user_score (tratamiento de tbd), cómputo de global_sales = na+eu+jp+other.

## Método
1.  **Carga y Preprocesamiento de Datos:**
    *   Carga del conjunto de datos en un DataFrame de pandas.
    *   Inspección inicial de tipos de datos y valores ausentes.
    *   Limpieza de nombres de columnas.
    *   Manejo de valores ausentes en columnas clave (`name`, `genre`, `year_of_release`).
    *   Conversión de `user_score` a tipo numérico, manejando los valores 'tbd'.
    *   Cálculo de las ventas totales para cada juego.

2.  **Análisis Exploratorio de Datos (EDA):**
    *   Análisis del número de juegos lanzados por año para comprender el crecimiento del mercado.
    *   Investigación de las ventas totales por plataforma para identificar los líderes del mercado.
    *   Análisis de la evolución anual de las ventas de las plataformas principales para comprender sus ciclos de vida.
    *   Selección y efinición de un período relevante (2010-2016) para análisis futuros basado en las tendencias de las plataformas.
    *   Examen de la distribución de las ventas globales por plataforma utilizando diagramas de caja.
    *   Cálculo y comparación de las ventas promedio y mediana por plataforma.
    *   Análisis de la relación entre las puntuaciones de críticos, usuarios y las ventas totales, centrándose en una plataforma popular (PS4) como ejemplo.
    *   Comparación de las ventas de los juegos más vendidos en diferentes plataformas.
    *   Análisis de la distribución general y métricas estadísticas de los juegos por género.

3.  **Perfil de Usuario Regional:**
    *   Identificación del Top 5 de las Plataformas y Géneros por cuota de mercado en Norteamérica, Europa y Japón.
    *   Análisis del impacto de las clasificaciones de los criticos en las ventas en cada región.
    *   Graficos de las preferencias regionales de plataformas, géneros y clasificaciones.

4.  **Pruebas de Hipótesis:**
    *   Prueba de la hipótesis de que las puntuaciones promedio de los usuarios para las plataformas Xbox One y PC son las mismas.
    *   Prueba de la hipótesis de que las puntuaciones promedio de los usuarios para los géneros Acción y Deportes son diferentes.
    *   Discusión del criterio estadístico utilizado para las pruebas de hipótesis.

5.  **Hallazgos clave:**
    *   Resumen de los hallazgos clave sobre los ciclos de vida de las plataformas, los factores que influyen en las ventas, los patrones de consumo regional y el rendimiento de los géneros.
    *   Recomendaciones ejecutables para la estrategia de la tienda Ice en 2017, enfocárse en plataformas clave, estrategias de género, aprovechamiento de reseñas y personalización regional del marketing.

## KPIs

*   Los ciclos de vida de las plataformas impactan significativamente en las ventas; PS4 y Xbox One fueron plataformas clave en la parte final del período de análisis.
*   Las puntuaciones de críticos muestran una correlación positiva moderada con las ventas, mientras que las de usuarios muestran una correlación más débil.
*   Existen diferencias regionales significativas en las preferencias de plataformas y géneros (por ejemplo, los juegos de Rol y las consolas portátiles son más populares en Japón).
*   Las clasificaciones de los criticos influyen en las ventas, particularmente en Norteamérica y Europa, donde los juegos con clasificación "M" tienen un fuerte rendimiento.
*   Las pruebas de hipótesis confirmaron diferencias en las puntuaciones de usuarios entre los géneros Acción y Deportes, mientras que no encontraron una diferencia estadísticamente significativa entre las puntuaciones de usuarios de Xbox One y PC en el período relevante.

## Recomendaciones para Ice

*   Priorizar el inventario y las campañas de marketing en plataformas de alto rendimiento como PS4 y Xbox One.
*   Adaptar las estrategias de género y los esfuerzos de marketing basados en las preferencias regionales (por ejemplo, enfatizar Acción/Shooter en NA/EU, Rol en JP).
*   Considerar las puntuaciones de críticos como un indicador útil del potencial de ventas de un juego.
*   Personalizar los mensajes de marketing y las promociones para cada región.

## Cómo Ejecutar el Código

1.  Clona este repositorio.
2.  Asegúrate de tener Python y las librerías necesarias instaladas (pandas, numpy, matplotlib, seaborn, scipy).
3.  Abre el Notebook Proyecto?Videojuegos en un entorno como Google Colab, JupyterLab o Jupyter Notebook o VS Code.
4.  Ejecuta las celdas secuencialmente.

Este proyecto tiene fines educativos y demuestra técnicas de análisis de datos aplicadas.

## Autor

Daniel Pineda


