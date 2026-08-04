# Selección de literatura para el paper de ArGos

La colección recuperada contiene 20 PDFs en `Paper/Recursos/`. El manuscrito usa
principalmente 17 fuentes que cubren el problema de investigación, la arquitectura
y los límites del sistema. La selección evita citar un paper solo porque está
disponible: cada referencia debe respaldar una afirmación concreta.

## Fuentes incorporadas

| Eje | Fuentes | Uso en el manuscrito |
|---|---|---|
| Descubrimiento EASM | ZMap; Censys | Escaneo a escala, medición responsable e indexación continua de servicios. |
| Escaneo web | Automatic Vulnerability Scanner; AI-Assisted Web Vulnerability Scanner | Diferenciar detección/crawling de la contribución de verificación y gobierno de ArGos. |
| Severidad y priorización | CVSS; análisis de CVSS v2; EPSS; survey de priorización; Vulnerability Management Chaining | Justificar el score transparente y, a la vez, declarar que aún faltan EPSS, KEV y criticidad del activo. |
| Agentes para SOC | ReAct; LLMs for SOC; AI-Augmented SOC | Situar el asistente como herramienta de consulta y explicación, no como fuente de verdad. |
| Prompt injection | Indirect Prompt Injection; Spotlighting; SecureCAI | Construir el modelo de amenaza para datos de escaneo controlados por atacantes y motivar el datamarking. |
| MCP | MCP Landscape; MCP at First Glance | Motivar interoperabilidad, autenticación por tool, scoping, auditoría y riesgos específicos de MCP. |

## Fuentes no centrales

- **An Integrated Development Environment for Synthesising Web Services**: no
  aborda EASM, verificación de vulnerabilidades, LLMs ni MCP; se excluye.
- **VulSlicer**: se concentra en detección estática mediante *code slicing*;
  ArGos evalúa superficie externa y no analiza código fuente en su pipeline actual.
- **WIVSS**: es un antecedente válido de ponderación de CVSS, pero el argumento
  ya queda cubierto por CVSS, EPSS, el survey de priorización y el chaining. Puede
  incorporarse si una versión extendida profundiza en la fórmula de scoring.

## Límite de evidencia

Las fuentes permiten justificar las decisiones de diseño y comparar enfoques.
No sustituyen una evaluación empírica propia. Por eso el paper reporta por separado
la validación del artefacto y deja como trabajo futuro la precisión de detección,
el rendimiento en escaneos longitudinales y la resistencia adversarial del asistente.
