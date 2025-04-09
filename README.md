# 🚌 Análisis de Movilidad Pública en Argentina (2024)

Este proyecto explora el uso del transporte público en Argentina durante el año 2024, utilizando datos abiertos procesados con PySpark en Databricks y visualizados en R Studio.

---

## ⚙️ Stack utilizado

- 🐍 Python
- 🔥 PySpark
- 🧠 Databricks Community Edition
- 📊 R Studio
- 📁 DBFS / CSV

---

## 🔄 Pipeline del proyecto

1. **Carga del dataset crudo** desde archivo `.csv` (`dat-ab-usos-2024.csv`) subido a DBFS.
2. **Limpieza de datos en PySpark**:
   - Conversión de fechas
   - Eliminación de valores nulos y códigos inválidos (`JN`, `SD`)
   - Normalización de columnas clave (`PROVINCIA`, `TIPO_TRANSPORTE`)
3. **Agrupación y transformación**:
   - Total de viajes por provincia, fecha y tipo de transporte
4. **Exportación del dataset final** como `.csv` desde Databricks.
5. **Visualización exploratoria** realizada con R (ggplot2).

---

## 📷 Vista del gráfico resumen

![Gráfico de viajes por provincia](/grafico_resumen.png)

---

## 📊 Resultados destacados

- **Buenos Aires** concentra la mayor parte del uso del transporte público en Argentina.
- **Desigualdad notable** en la distribución de viajes entre provincias.
- Dataset final apto para dashboards, modelos predictivos o cruces con otras fuentes (salud, seguridad, clima).

---

## 📁 Estructura del proyecto

- transporte-argentina-2024/
  - resumen_transporte.csv
  - grafico_resumen.png
  - README.md
    
---

## 🧠 Qué aprendí

- Cómo estructurar un proyecto de análisis de datos de punta a punta.
- Uso práctico de PySpark para ETL en grandes volúmenes de datos.
- Carga y procesamiento de archivos en Databricks (DBFS).
- Visualización y publicación de dashboards en Power BI Online.

---

## 🧑‍💻 Autor

Juan Ignacio Algarin  
Estudiante de Lic. en Ciencia de Datos – Universidad Nacional de San Martín (UNSAM)  
📧 juanalgarin00@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/juan-ignacio-algarin-0167b018b/)

---

## 📌 Dataset original

- Fuente: [datos.gob.ar – Cantidad de transacciones SUBE por fecha](https://datos.gob.ar/dataset/transporte-sube---cantidad-transacciones-usos-por-fecha/archivo/transporte_c7dad6d8-8fe4-449e-82c9-18ed8574eae8)
