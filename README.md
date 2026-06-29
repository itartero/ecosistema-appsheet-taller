# 🏭 Ecosistema Digital de Gestión: Taller Circularidad (AppSheet)

![AppSheet](https://img.shields.io/badge/AppSheet-34A853?style=for-the-badge&logo=google&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Data Architecture](https://img.shields.io/badge/Relational_Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

Un ecosistema integral desarrollado con tecnología No-Code (AppSheet) para centralizar, digitalizar y automatizar la operativa del Taller Regional de Economía Circular. Este proyecto transforma flujos de trabajo manuales y bases de datos aisladas en una arquitectura relacional única y escalable.

---

## 🎯 El Reto
Antes de la implementación, el taller operaba con procesos manuales y hojas de cálculo desconectadas. Esto generaba cuellos de botella en la recepción de productos, pérdida de trazabilidad en los componentes (piezas en espera) y una gestión ineficiente del espacio en el almacén (lineal). La falta de datos estructurados impedía la toma de decisiones ágil y la monitorización de la productividad.

## 💡 La Solución
Diseño y desarrollo de una aplicación relacional con AppSheet que abarca todo el ciclo de vida del producto en el taller. La solución no solo actúa como interfaz de usuario (Front-end), sino que orquesta una base de datos relacional (Back-end) estructurada en tres grandes módulos funcionales.

---

## 📈 Impacto en Negocio (KPIs)

* 🚀 **+163% de Productividad:** Incremento masivo en la velocidad de registro e ingesta de productos reacondicionados en el sistema.
* ⏱️ **-90% Tiempo de Búsqueda:** Reducción drástica en los tiempos de localización y guardado de componentes gracias al módulo "Lineal" y su lógica de ubicaciones inteligentes.
* 📊 **Gobernanza del Dato:** Eliminación de los silos de información, logrando un 100% de trazabilidad desde que un artículo llega de una tienda hasta que se repara y almacena.

---

## 🗄️ Arquitectura de Datos (Data Modeling)

El modelo de datos se sostiene sobre un esquema de tablas relacionales divididas en tres áreas core:

### 1. Módulo TRATAMIENTO (Flujo Operativo)
Gestiona el corazón de las operaciones técnicas y el estado de los activos.
* `Registro_Productos` / `Registro Máquinas Montadas` / `Electrónica`
* `Espera_Piezas` y `Solicitudes_Compra` (Trazabilidad de recambios)
* `Tiendas` y `Colaboradores` (Asignación y orígenes)

### 2. Módulo LINEAL (Control de Inventario)
Sistema inteligente de gestión de almacén.
* `Lineal_Maestro` y `Articulos` (Catálogo core)
* `Ubicaciones_Borradas` y `Contadores` (Control de stock espacial)
* `Buscador_Lineal` (Querying rápido de ubicaciones)

### 3. Módulo EMPLEABILIDAD (Business Intelligence)
Orientado a la medición del rendimiento y la gestión de la capacidad operativa.
* `Dashboard` y `Inicio` (Vistas ejecutivas)
* `Empleabilidad` (Registro de Tiempos Teóricos - TT y cargas de trabajo)

---

## 📸 Interfaz y Casos de Uso

*(Nota: Los datos mostrados en las siguientes capturas han sido anonimizados o alterados para proteger la confidencialidad de la empresa).*

### 1. Registro Ágil de Productos
> <img width="1902" height="905" alt="image" src="https://github.com/user-attachments/assets/be8029bd-c1eb-4a3c-a317-23fd3bcba0eb" />
*Formulario optimizado para reducir fricción en la entrada de datos por parte de los técnicos.*

### 2. Gestión de Inventario (Módulo Lineal)
> <img width="1902" height="909" alt="image" src="https://github.com/user-attachments/assets/6feeba8b-809d-4f8f-8e02-0907623b8f17" />
*Sistema de control espacial que redujo los tiempos de búsqueda en un 90%.*

### 3. Control de Empleabilidad (Dashboard Integrado)
> <img width="1902" height="911" alt="image" src="https://github.com/user-attachments/assets/43291621-b2a9-470e-a3d5-ab0c62f19e58" />
*Vista consolidada para la toma de decisiones diaria sobre la carga del taller.*

---

## 🚀 Próximos Pasos (Roadmap)
Como parte de mi evolución hacia perfiles de **Data Science & Big Data**, el siguiente paso arquitectónico para este ecosistema es la migración de las tablas maestras a **Google BigQuery** para dotarlo de mayor capacidad transaccional y la explotación de sus datos mediante plataformas de visualización avanzada (**Tableau / Looker Studio**).
