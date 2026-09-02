# ============================================
# BOT DE VENTAS - Script completo
# Ejecuten y respondan las preguntas en su README
# ============================================
# --------------------------------------------
# PARTE 1: Leer los archivos
# --------------------------------------------
# PREGUNTA 1 (para su README): que hace glob.glob()?
#Sirve para buscar archivos que coincidan con un patrón específico dentro de una carpeta. Por ejemplo, en la linea de codigo: glob.glob("data/sucursal_*.csv").
#Busca todos los archivos CSV que estén dentro de la carpeta data y cuyo nombre comience por sucursal_.
# --------------------------------------------
# PARTE 2: Consolidar y renombrar columnas
# --------------------------------------------
# PREGUNTA 2: que hace pd.concat()? por que se ejecuta dos veces?
#sirve para unir o concatenar varios DataFrames en uno solo.
#Se ejecuta dos veces porque el código tiene dos procesos diferentes:
#1.Se unen los archivos inicialmente, antes de cambiar los nombres de las columnas.
#2.Después de renombrar las columnas de cada DataFrame, se vuelven a unir para crear el consolidado definitivo.
# PREGUNTA 3: que hace enumerate()? por que se necesita aqui (i)?
#enumerate() permite recorrer una lista obteniendo dos cosas al mismo tiempo: La posición o índice del elemento y El elemento de la lista.
#i representa la posición y df representa el DataFrame.
# --------------------------------------------
# PARTE 3: Limpieza
# --------------------------------------------
# PREGUNTA 4: que hace drop_duplicates()? que hace fillna()?
#drop_duplicates() Sirve para eliminar filas duplicadas de un DataFrame.
#fillna() Sirve para rellenar valores faltantes o NaN.
# --------------------------------------------
# PARTE 4: Analisis y graficos
# --------------------------------------------
# PREGUNTA 5: que hace groupby()? cual es la diferencia entre el 
# grafico de barras y el de torta, cuando usar cada uno?
#groupby() sirve para agrupar los datos según una columna y después realizar operaciones sobre esos grupos.
#Gráfico de barras: Permite comparar fácilmente diferentes categorías o valores.
#Gráfico de torta: El gráfico de torta muestra cómo se distribuye un total entre diferentes partes.