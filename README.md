# Plantilla del Curso: Deep Learning

Este repositorio es una **plantilla** para el proyecto final del curso de *Advanced Machine Learning*.


Información del Proyecto
---------
Nombre del Estudiant: Kevin Pierre Barra Torres
Título del Proyecto: Predicción y análisis de Asistencia (Venue) para Artistas en conciertos.
Fecha de Entrega: 04/05/26.
Profesor: Carlos Mariño

---

## Pasos para usar esta plantilla (OBLIGATORIO)

### 1. Crear tu repositorio personal

1. Ir a este repositorio plantilla
2. Hacer clic en el botón verde **“Use this template”**
3. Crear un nuevo repositorio con el nombre:

   `AML-Final-Apellido-Nombre`

Ejemplo: `AML-Final-Marino-C.`

---

### 2. Trabajar SOLO en el notebook desde Colab

1. En tu repositorio, entrar a la carpeta `notebooks/`
2. Abrir el archivo: `final_project.ipynb`
3. Hacer clic en **“Open in Colab”**
4. Desarrollar todo tu proyecto dentro de este notebook

No es necesario usar comandos de git ni terminal.

---

### 3. Guardar cambios directamente en GitHub

Dentro de Colab:

* Ir a **File → Save a copy in GitHub**
* Seleccionar tu repositorio personal
* Confirmar sobrescribir el notebook

De esta forma, tu trabajo quedará guardado automáticamente en GitHub.

---

## Estructura del repositorio (NO modificar)

* `notebooks/` → Notebook principal del proyecto
* `src/` → Código auxiliar (opcional)
* `data/` → Solo instrucciones del dataset (no subir datos grandes)
* `results/` → Resultados y métricas
* `figures/` → Gráficos generados
* `report/` → Reporte final (PDF o Markdown)

Los estudiantes deben principalmente trabajar en:
`notebooks/final_project.ipynb`

---

## Reglas importantes

* No subir datasets grandes o datos sensibles
* El notebook debe poder ejecutarse en Colab
* Incluir visualizaciones y evaluación del modelo
* Mantener el código organizado y reproducible

---

## Entrega final

Cada estudiante deberá enviar:

1. El enlace de su repositorio en GitHub
2. El notebook final completamente ejecutable
3. (Opcional) un tag final: `v1.0-final`

---

10. Conclusiones y Recomendaciones de Negocio

10.1 Resumen de Resultados
Instrucciones: Proporcione un resumen ejecutivo de los resultados:

El proyecto logró desarrollar un modelo predictivo basado en Redes Neuronales Profundas (PyTorch) capaz de estimar la asistencia a conciertos utilizando métricas de plataformas de streaming y factores de mercado local. Tras enfrentar retos iniciales de escala, la implementación de una transformación logarítmica en la variable objetivo permitió estabilizar las predicciones, logrando que el modelo identifique correctamente órdenes de magnitud en la asistencia para una variedad de artistas globales y locales.

10.2 Conclusiones
Instrucciones: Liste las conclusiones principales:

Efectividad del Escalamiento Logarítmico: La normalización de datos masivos mediante np.log1p resultó ser el factor crítico para el éxito del modelo, permitiendo que una arquitectura de red sencilla aprendiera patrones en un dataset pequeño sin colapsar ante valores extremos.
Correlación Digital-Física: Se confirma que los "Oyentes Mensuales" y los "Seguidores" son predictores potentes de asistencia, pero su impacto no es lineal; el modelo demuestra que el crecimiento de la audiencia física sigue una curva exponencial que la IA puede mapear con precisión creciente.
10.3 Recomendaciones de Negocio
Instrucciones: Proporcione recomendaciones accionables basadas en los resultados:

Recomendaciones a Corto Plazo:

Validación de Recintos: Utilizar las predicciones del modelo como una "segunda opinión" técnica antes de firmar contratos de alquiler de recintos para artistas nuevos.
Ajuste de Precios: Emplear la "Asistencia Predictiva" para estimar el punto de equilibrio (break-even) y ajustar el precio de las entradas en etapas tempranas de preventa.
Recomendaciones a Mediano Plazo:

Optimización de Giras: Identificar mercados locales donde la IA prediga una asistencia mayor a la esperada subjetivamente, priorizando esas ciudades en la logística de la gira.
Monitoreo de Tendencias: Integrar una actualización semanal de datos de streaming para observar cómo la predicción de asistencia evoluciona antes de que se anuncie oficialmente el evento.
Recomendaciones a Largo Plazo:

Sistema de Recomendación de Inversión: Desarrollar un tablero de control (Dashboard) que califique el "riesgo de inversión" por artista basado en la brecha entre su costo de contratación y la asistencia predicha por la IA.
Expansión Multi-Mercado: Escalar el modelo para incluir datos de múltiples países, permitiendo predecir el éxito de artistas internacionales en mercados donde nunca se han presentado.
10.4 Limitaciones del Estudio
Instrucciones: Identifique las limitaciones de su análisis:

Tamaño del Dataset: El análisis se limitó a una muestra de aproximadamente 100 artistas, lo que restringe la capacidad de la red neuronal para aprender patrones más sutiles en nichos musicales específicos.
Variables Externas No Consideradas: El modelo no incluye factores dinámicos como la estacionalidad (fechas festivas), la competencia con otros eventos simultáneos o el precio de los boletos, los cuales influyen directamente en la asistencia final.
10.5 Trabajo Futuro
Instrucciones: Proponga líneas de investigación futura:

Implementación de Modelos de Ensamble: Evaluar el rendimiento de algoritmos como XGBoost o Random Forest para comparar su precisión frente a la red neuronal actual en entornos de datos limitados.
Ingeniería de Características Avanzada: Incorporar nuevas variables como el sentimiento en redes sociales (Twitter/Instagram) y la frecuencia de lanzamientos recientes para capturar el "momento" o tendencia actual del artista.
11. Referencias
Instrucciones: Liste todas las referencias utilizadas (formato APA):

Pollstar. (2026). Pollstar Data Cloud: Live entertainment box office database. https://www.pollstar.com/

Spotify. (2026). Spotify for Artists: Audience analytics and monthly listeners data. https://artists.spotify.com/

Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning. MIT Press. (Capítulos sobre Redes Neuronales Multicapa y Optimización).

Harris, C. R., Millman, K. J., van der Walt, S. J., Gommers, R., Virtanen, P., Cournapeau, D., ... & Oliphant, T. E. (2020). Array programming with NumPy. Nature, 585(7825), 357-362. (Referencia para el uso de log1p y transformaciones matemáticas).
