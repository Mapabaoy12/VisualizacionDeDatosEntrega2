# StreamView Analytics: Estrategia y Visualización de Datos

## Descripción del Proyecto

Este proyecto fue desarrollado para StreamView Analytics, una plataforma internacional de streaming digital operando en Latinoamérica. Ante un crecimiento acelerado y un mercado altamente competitivo, la organización enfrentaba problemas de fragmentación analítica, silos de información y decisiones basadas en métricas parciales.

El objetivo principal de este proyecto es transformar grandes volúmenes de datos en información útil mediante la exploración, diseño e implementación de dashboards interactivos. Estas herramientas visuales están diseñadas para apoyar la toma de decisiones estratégicas, eliminar sesgos estadísticos y detectar oportunidades de negocio reales (como la activación de contenido inactivo de alta calidad).

## Objetivos

* Unificar criterios analíticos: Consolidar métricas aisladas en un modelo de datos centralizado.
* Caracterizar el catálogo audiovisual: Analizar la distribución por país, rating, género, popularidad y Retorno de Inversión (ROI).
* Corregir sesgos de información: Implementar percentiles segmentados para comparar de forma justa el rendimiento de películas vs. series.
* Identificar Oportunidades ("Joyas Ocultas"): Detectar contenido de alta valoración pero baja exposición comercial para optimizar el presupuesto de marketing.
* Construir Dashboards Especializados: Desarrollar tableros adaptados a perfiles Ejecutivos/Financieros y de Marketing/Operaciones, aplicando principios de percepción visual (patrón de lectura en "Z").

## Fuentes de Datos

El proyecto integra bases de datos corporativas enriquecidas con metadatos cinematográficos internacionales (TMDB):

1. Dataset de Películas (Netflix Movies Detailed up to 2025): 16.000 registros.
2. Dataset de Series (Netflix TV Shows Detailed up to 2025): 16.000 registros.

Procesamiento y Limpieza:

* Integración y normalización de columnas.
* Manejo de valores atípicos y nulos (especialmente en métricas descriptivas y financieras).
* Implementación de sentencias DAX estrictas en Power BI para evitar falsos positivos matemáticos en producciones sin datos de recaudación válidos.

## Hallazgos Principales

* Cobertura Financiera y Rentabilidad: Actualmente, el catálogo cuenta con una cobertura financiera verificada del 45,76%. Sobre esta base, el Retorno de Inversión (ROI) global es de 2.93, demostrando que el portafolio casi triplica el capital invertido.
* Dominio del Nicho: El 71,50% del catálogo se considera contenido de nicho, dirigido a audiencias hiper-específicas.
* Supremacía del Drama: El género dramático es el núcleo seguro de la plataforma, liderando consistentemente en volumen de interacción y retención de calidad.
* Corrección de Sesgo Estadístico: Se detectó una distorsión algorítmica donde las series acumulaban popularidades de hasta 6.800 unidades frente a las 3.800 de las películas. Esto se solucionó aplicando un modelo analítico de Percentiles Segmentados.

### El Descubrimiento Clave: Las "Joyas Ocultas"

Se identificó un segmento estratégico de 1.301 producciones (447 películas y 854 series) que representan una oportunidad comercial a costo cero.

* Criterio: Títulos con calidad de excelencia (vote_average >= 7.5 y vote_count >= 30), pero con popularidad por debajo de la mediana del formato.
* Pivote Geográfico (Series): Fuerte hegemonía asiática. Japón y Corea del Sur son motores absolutos de calidad desaprovechada en formatos de animación, drama y ciencia ficción.
* Pivote Temático (Películas): La mayor eficiencia de calidad reside en Documentales y producciones Musicales.

## Indicadores Clave de Rendimiento (KPIs)

Para monitorear el éxito de las decisiones estratégicas, se definieron los siguientes KPIs:

1. Cobertura de Datos Financieros:
   * Actual: 45,76%.
   * Meta: Alcanzar un 85% de cobertura en 12 meses (exigiendo transparencia en nuevos contratos).

2. Retorno de Inversión (ROI):
   * Actual: 2.93.
   * Meta: Incrementar a >= 3.5 en 12 meses priorizando licencias de bajo costo y alta retención.

3. Conversión de Joyas Ocultas:
   * Meta: Traccionar al menos al 15% de los títulos "Por Descubrir" hacia percentiles de alta popularidad (sobre el 75%) mediante campañas dirigidas en redes sociales.

## Estructura de Dashboards

La arquitectura visual en Power BI se basó en reducir la carga cognitiva y facilitar la acción:

### 1. Dashboard Ejecutivo (Finanzas y Adquisiciones)
* Enfoque: Riesgo, rentabilidad histórica y evolución del catálogo.
* Componentes: Gráfico de áreas apiladas para monitorear la adquisición de contenido, barras agrupadas para el potencial por género, y medidores (Gauge) centralizados para auditar el ROI y la cobertura de datos en tiempo real.

### 2. Dashboard de Marketing (Operaciones y Crecimiento)
* Enfoque: Acción directa y maximización de retención.
* Componentes: Se eliminó el factor costos. Su núcleo es un gráfico de dispersión libre de sesgos (basado en percentiles) que aísla visualmente el cuadrante de las "Joyas Ocultas". Incluye una matriz accionable con los nombres exactos de los títulos a promocionar.

## Conclusión y Recomendaciones

La consolidación de datos demostró que StreamView Analytics opera exitosamente bajo un modelo "Long Tail". La principal oportunidad comercial no reside en adquirir costosos blockbusters, sino en rentabilizar el inventario inactivo mediante las siguientes acciones:

* Marketing: Redirigir el presupuesto publicitario hacia las "Joyas Ocultas" (especialmente asiáticas y documentales) para generar retención a costo de adquisición cero.
* Adquisiciones: Mantener el género Drama como núcleo de seguridad e invertir en licencias internacionales de costo controlado para alcanzar el ROI proyectado.
* Gobernanza de Datos: Exigir reportes financieros transparentes a las distribuidoras en las renovaciones de contratos para superar la actual limitación del 45,76% de visibilidad económica.

Proyecto desarrollado para la asignatura de Visualización de Datos (ADY 1104-001D) - Duoc UC Concepción.
