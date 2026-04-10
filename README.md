# 📊 Proyecto de Análisis de Ventas con SQL Server

## 🚀 Descripción

Este proyecto tiene como objetivo analizar datos de ventas para identificar tendencias, productos más vendidos y oportunidades de mejora en el negocio.

Se desarrollaron consultas avanzadas en **T-SQL** para transformar y analizar la información, generando insights clave para la toma de decisiones.

---

## 🎯 Objetivos

* Analizar el comportamiento de ventas por mes
* Identificar los productos más vendidos
* Detectar productos con bajo rendimiento
* Generar reportes para la toma de decisiones

---

## 🛠️ Tecnologías utilizadas

* SQL Server
* T-SQL
* Excel
* Power BI

---

## 📂 Estructura del proyecto

```
📁 analisis-ventas
 ┣ 📂 datasets
 ┣ 📂 scripts-sql
 ┣ 📂 dashboards
 ┗ README.md
```

---

## 📊 Análisis realizado

### 🔹 Ventas mensuales

Consulta para obtener ventas por mes:

```sql
SELECT 
    MONTH(fecha) AS mes,
    SUM(total) AS ventas_totales
FROM ventas
GROUP BY MONTH(fecha)
ORDER BY mes;
```

---

### 🔹 Productos más vendidos

```sql
SELECT 
    producto,
    SUM(cantidad) AS total_vendido
FROM ventas
GROUP BY producto
ORDER BY total_vendido DESC;
```

---

## 📈 Resultados

* El producto más vendido fueron los **zapatos**
* Se observó un incremento en ventas en el mes de febrero
* Las **gorras** presentan baja rotación, se recomienda promoción

---

## 📸 Evidencia

*Aquí puedes agregar capturas de tus dashboards o resultados*

---

## 💡 Conclusiones

El análisis permitió identificar oportunidades de mejora en la estrategia comercial, enfocándose en productos con menor rendimiento.

---

## 👩‍💻 Sobre mí

Ingeniera de Sistemas en formación con interés en el área de **Ingeniería de Datos**.

🔹 Habilidades:

* SQL (intermedio)
* Análisis de datos
* Visualización (Power BI)

---

## 📬 Contacto

* LinkedIn: *agrega tu link aquí*
* GitHub: *tu usuario*

---

⭐ Si te gustó este proyecto, ¡no olvides darle un star!
