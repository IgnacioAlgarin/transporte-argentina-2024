# 🚌 Análisis de Movilidad Pública en Argentina (2024)

Este proyecto explora el uso del transporte público en Argentina durante el año 2024, utilizando datos abiertos procesados con PySpark en Databricks y visualizados en Power BI Online.

---

## ⚙️ Stack utilizado

- 🐍 Python
- 🔥 PySpark
- 🧠 Databricks Community Edition
- 📊 Power BI Online
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
5. **Visualización interactiva** con Power BI Online.

---

## 📊 Resultados destacados

- **Buenos Aires** concentra la mayor parte del uso del transporte público en Argentina.
- **Desigualdad notable** en la distribución de viajes entre provincias.
- Dataset final apto para dashboards, modelos predictivos o cruces con otras fuentes (salud, seguridad, clima).

---

## 📁 Estructura del proyecto

- transporte-argentina-2024/
  - resumen_transporte.csv
  - dashboard_powerbi_online.png (opcional)
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

- Fuente: [Transporte público de Argentina – datos.gob.ar](https://datos.gob.ar)
