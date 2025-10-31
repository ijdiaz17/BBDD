# 📚 Proyecto BBDD - Mesa 3

## 📌 Descripción del proyecto
Este proyecto tiene como objetivo la **creación, modelado y gestión de una base de datos relacional** que representa un entorno académico.  
La base de datos incluye entidades como **alumnos, profesores, cursos, campus, proyectos y calificaciones**, y busca aplicar principios de diseño de bases de datos, normalización y relaciones entre tablas.

El trabajo se desarrolló íntegramente en **Python** utilizando **SQLite** como sistema gestor de base de datos.

---

## 🧱 Estructura del proyecto

El notebook principal es:

```
PROYECTO_BBDD_MESA3.ipynb
```

### Contenido del notebook:

1. **Importación de librerías**  
   Carga de las librerías necesarias para la manipulación de datos y conexión con la base de datos.

2. **Conexión a la base de datos (SQLite)**  
   Creación o conexión a una base de datos local utilizando la librería `sqlite3`.

3. **Importación de datos (CSV)**  
   Carga de archivos `.csv` que contienen la información de partida (alumnos, profesores, cursos, etc.).

4. **Creación de tablas**  
   - Tablas de dimensiones: `alumnos`, `profesores`, `verticales`, `campus`, `promociones`, `proyectos`.  
   - Tablas dependientes: relaciones intermedias entre entidades.  
   - Tabla central y tablas puente para modelar relaciones *muchos a muchos*.  
   - Tabla de hechos: contiene la información de calificaciones y matrículas.

5. **Inserción de datos**  
   Inserción manual y/o automatizada de los datos en las tablas creadas.

6. **Consultas de comprobación**  
   Ejecución de consultas SQL para verificar el correcto funcionamiento de las relaciones entre tablas.

---

## 🧰 Tecnologías utilizadas

- **Python 3.x**
- **SQLite3**
- **Pandas**
- **CSV (archivos fuente de datos)**
- **Jupyter Notebook / VSCode**

---

## ⚙️ Instalación y ejecución

1. Clonar este repositorio:
   ```bash
   git clone https://github.com/tu_usuario/PROYECTO_BBDD_MESA3.git
   ```

2. Instalar las dependencias necesarias:
   ```bash
   pip install pandas
   ```

3. Abrir el notebook en Jupyter o VSCode:
   ```bash
   jupyter notebook PROYECTO_BBDD_MESA3.ipynb
   ```

4. Ejecutar las celdas en orden para crear y poblar la base de datos.

---

## 🧩 Modelo de datos (resumen)

El modelo sigue un esquema tipo **estrella (star schema)** con:

- **Tablas de dimensiones:** información descriptiva (alumnos, profesores, etc.)
- **Tablas de hechos:** registros transaccionales (matrículas, calificaciones)
- **Tablas puente:** relaciones entre dimensiones y hechos.

---

## 📊 Resultados y comprobaciones

- Se logra la creación exitosa de todas las tablas del modelo.  
- Las consultas SQL permiten comprobar la consistencia e integridad de los datos.  
- Se valida la correcta relación entre entidades clave (alumnos ↔ cursos ↔ profesores).

---

## 👥 Autores

**Equipo Mesa 3**  
Proyecto realizado como parte del módulo de **Bases de Datos** del bootcamp de Data Science en *The Bridge*.

---

## 🗂️ Licencia

Este proyecto se distribuye bajo la licencia **MIT**.
