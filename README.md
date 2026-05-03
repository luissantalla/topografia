Esta herramienta, denominada LAS → DXF · Topografía, es una aplicación web especializada en el procesamiento de nubes de puntos LiDAR (archivos .LAS) para la generación de cartografía técnica, específicamente curvas de nivel y delimitación de parcelas.
¿Para qué sirve?
Su función principal es convertir datos brutos de escaneo láser (LiDAR) en archivos vectoriales de CAD (.DXF) que pueden ser utilizados en programas como AutoCAD, QGIS o Civil 3D. Permite filtrar el terreno, suavizar las líneas y superponer información catastral para obtener un plano topográfico preciso de una zona específica.
¿Qué se puede conseguir con ella?
Visualización de nubes de puntos: Ver la densidad y clasificación de los puntos (suelo, vegetación, edificios).
Curvas de nivel personalizadas: Generar curvas maestras y normales con intervalos (equidistancia) ajustables.
Recortes precisos: Aislar una zona de interés mediante recortes rectangulares o poligonales.
Integración catastral: Superponer archivos DXF de catastro para alinear la nube de puntos con las lindes de las parcelas.
Mediciones: Calcular distancias y áreas directamente sobre la nube de puntos.
Exportación profesional: Obtener un archivo DXF que incluye las curvas de nivel, la geometría del catastro y las huellas de edificación detectadas.
Manual de Uso: Paso a Paso
Para obtener un resultado óptimo, sigue estos pasos en orden:
Paso 1: Carga de archivos
Archivo LAS: Arrastra tu archivo de nube de puntos al recuadro superior izquierdo (icono de antena 📡). La herramienta cargará una vista previa y mostrará las estadísticas de los puntos.
Archivo DXF (Opcional): Si tienes el archivo del catastro o de la parcela, cárgalo en la sección "Catastro .DXF". La herramienta te preguntará si quieres usar el borde de la parcela como recorte automático; esto es muy útil para centrarte solo en el área de trabajo.
Paso 2: Definición del área de trabajo (Recorte)
Si no has usado el recorte automático del DXF, utiliza las herramientas de la sección "Recorte":
Rectangular: Haz clic y arrastra sobre el mapa para definir un área cuadrada.
Poligonal: Haz clics sucesivos para dibujar una forma irregular. Haz doble clic para cerrar el polígono.
Nota: Recortar el área mejora significativamente la velocidad de procesamiento y la limpieza del resultado final.
Paso 3: Selección de Clases
En el panel "Clases detectadas", asegúrate de que la clase "Suelo / Terreno" esté marcada.
Si deseas que la vegetación o los edificios aparezcan en la previsualización, actívalos, pero recuerda que para generar las curvas de nivel, el algoritmo suele priorizar solo los puntos de "Suelo" para evitar errores de elevación causados por árboles o techos.
Paso 4: Configuración de parámetros de proceso
Ajusta los valores en la sección "Proceso":
Equidistancia (m): Define cada cuántos metros quieres una curva de nivel (ej. 1m para detalle alto, 5m para terreno amplio).
Resolución (m): Es el tamaño de la rejilla de cálculo. Una resolución de 1 o 2 metros suele ser ideal. Valores muy bajos pueden generar ruido si la nube de puntos no es densa.
Suavizado (pasadas): Ajusta cuántas veces se "pulirán" las líneas. Un valor de 3 a 5 suele dar curvas estéticas y fluidas sin perder precisión topográfica.
Paso 5: Generación y Exportación
Haz clic en "Generar curvas de nivel". Verás una barra de progreso mientras se calcula la interpolación del terreno.
Una vez generadas, aparecerán en el mapa (verdes las normales, naranjas las maestras).
Si estás satisfecho, haz clic en el botón naranja "Exportar DXF" al final del panel lateral para descargar el archivo final.
Consejos para un resultado excelente
Limpieza de ruido: Si el terreno tiene muchas irregularidades extrañas, aumenta el número de pasadas de suavizado.

Precisión X,Y: Usa el buscador de coordenadas en la parte inferior derecha si necesitas verificar un punto exacto de un acta de replanteo o deslinde.

Medición previa: Usa la herramienta de "Medición" antes de procesar para verificar que las dimensiones del terreno coinciden con tus expectativas.
