# Resumen-Materia
Este repositorio contiene los resúmenes principales de la materia, junto con ejemplos prácticos relacionados con la gestión de bases de datos y el uso de Python para trabajar con tablas. Además, incluye el código SQL y Python correspondiente a la tabla de "Métricas de Progreso".

Proposito del proyecto
El objetivo de este proyecto es demostrar la integración de conceptos teóricos y prácticos, como:
- **Ingeniería de Requerimientos**: Identificación y definición de necesidades.
- **Gestión de Bases de Datos**: Creación, manipulación y consulta de datos.
- **Programación en Python**: Automatización de operaciones en bases de datos.

Este repositorio también está diseñado para aprender a usar herramientas de control de versiones como **Git** y **GitHub**, y para alojar contenido como una página web mediante **GitHub Pages**.

conceptos clave de la materia:
  - Ingeniería de Software.
   - Metodologías Ágiles.
   - Bases de Datos Relacionales.
   - Programación con Python.
     Este repositorio se aloja como una página web pública que puedes visitar en:
      [https://<brayan3229>.github.io/resumen-materia]()

     codigo de la tabla asignada
     CREATE TABLE progress_metrics (
    metric_id INTEGER PRIMARY KEY AUTOINCREMENT,
    plan_id INTEGER,
    metric_type TEXT, -- 'financial', 'time', 'impact'
    current_value DECIMAL(10,2),
    target_value DECIMAL(10,2),
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (plan_id) REFERENCES strategic_plan(plan_id)
);
