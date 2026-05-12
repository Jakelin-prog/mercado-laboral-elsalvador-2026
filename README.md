# Análisis de Habilidades del Mercado Laboral — El Salvador 2026

**¿Qué habilidades está pidiendo realmente el mercado laboral en El Salvador?**

Este proyecto responde esa pregunta con datos reales extraídos de LinkedIn Jobs El Salvador en mayo de 2026. El análisis identifica las habilidades más demandadas, las categoriza y revela brechas entre lo que el mercado necesita y lo que la formación universitaria tradicional está entregando.

## Contexto y motivación

En LinkedIn es frecuente encontrar debate sobre las dificultades para encontrar empleo. Se culpa a los reclutadores, a las plataformas, a los requisitos exagerados. Pero hay una conversación menos frecuente: **¿qué responsabilidad tienen las instituciones educativas en esta desconexión?**

Este análisis surge de esa pregunta. El objetivo no es señalar culpables, sino generar evidencia que permita una conversación más informada sobre el futuro de la formación profesional en El Salvador.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `README.md` | Este documento |
| `dataset_linkedin.json` | Dataset original extraído de LinkedIn (430 ofertas) |
| `analisis_habilidades_sv.xlsx` | Resultados del análisis con ranking, gráficos y datos por categoría |
| `analisis_habilidades.ipynb` | Notebook con el código completo y los hallazgos documentados |

---

## Metodología

### Fuente de datos
- **Plataforma:** LinkedIn Jobs El Salvador (`sv.linkedin.com/jobs`)
- **Herramienta de extracción:** Apify — LinkedIn Jobs Scraper
- **Fecha de extracción:** 12 de mayo de 2026
- **Total de ofertas:** 430 publicaciones activas

### Proceso de análisis
1. **Extracción:** Web scraping de ofertas activas en LinkedIn El Salvador
2. **Limpieza:** Normalización de texto (minúsculas, eliminación de vacíos)
3. **Detección de habilidades:** Búsqueda de palabras clave por habilidad usando un diccionario de 23 competencias
4. **Cuantificación:** Conteo de frecuencia absoluta y relativa por habilidad
5. **Categorización:** Agrupación en 4 categorías (Técnica-Datos, Técnica-Negocios, Habilidades Blandas, Formación)
6. **Visualización:** Exportación a Excel con gráficos y análisis por industria

### Herramientas
- **Python 3** — pandas, collections
- **Apify** — extracción de datos
- **openpyxl** — generación del reporte en Excel

---

## Hallazgos principales

### Top 5 habilidades más demandadas

| # | Habilidad | Frecuencia | % de ofertas |
|---|---|---|---|
| 1 | Excel / Hojas de cálculo | 196 | 45.6% |
| 2 | Licenciatura / Universidad | 146 | 34.0% |
| 3 | Ventas / CRM | 124 | 28.8% |
| 4 | Experiencia requerida | 94 | 21.9% |
| 5 | Logística / Supply Chain | 92 | 21.4% |

### Hallazgos que llaman la atención

- **SAP/ERP (19.8%) supera a Python (2.6%) y Análisis de datos (6.5%)** — el mercado tradicional sigue dominando sobre el perfil tech
- **Inglés aparece solo en el 16.3%** de las ofertas — baja para un mercado que aspira a conectarse con la economía global
- **Power BI / Tableau: 5.8%** — las herramientas de visualización de datos tienen demanda incipiente pero creciente
- **Inteligencia Artificial: menos del 3%** — el mercado todavía no ha absorbido el discurso sobre IA en sus requisitos formales

### Distribución por categoría

| Categoría | % del total de menciones |
|---|---|
| Habilidades Blandas | 34% |
| Técnica - Negocios | 28% |
| Formación / Experiencia | 21% |
| Técnica - Datos y Tecnología | 17% |

---

## 💡 Interpretación

Las habilidades de datos y tecnología representan apenas el 17% de las menciones totales, a pesar de ser las más asociadas con empleabilidad futura. Esto sugiere dos lecturas posibles:

1. **El mercado está rezagado** respecto a las tendencias globales y aún no ha actualizado sus perfiles de puesto
2. **Las instituciones educativas no han generado suficiente oferta** de talento en estas áreas como para que las empresas lo incorporen naturalmente en sus requisitos

Ambas lecturas apuntan al mismo lugar: existe una brecha estructural entre la formación que se está ofreciendo y las habilidades que el mercado — presente y futuro — va a necesitar.

---

## Limitaciones

- Los datos provienen de una sola fuente (LinkedIn), que tiende a sobrerrepresentar sectores formales y empresas medianas-grandes
- La detección de habilidades se basa en palabras clave predefinidas; habilidades descritas con terminología no convencional pueden no haberse capturado
- La muestra corresponde a un momento específico (mayo 2026) y puede no reflejar variaciones estacionales

---

## Autora

**Jakelin Rivera**
Analista de datos | MBA — INCAE Business School
El Salvador


## Licencia

Este proyecto es de uso libre para fines educativos y de investigación. Si usas estos datos o metodología, por favor cita la fuente.
