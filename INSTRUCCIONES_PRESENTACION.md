# INSTRUCCIONES Y GUÍA DE TRABAJO — PRESENTACIÓN SPIROSCAN AI (NIVEL 1 Y NIVEL 2)

Este repositorio contiene la base de contenido y las directrices para continuar con la elaboración y diseño de las diapositivas de la presentación de producto **SpiroScan AI (VitalSync)**.

---

## 1. Contexto y Propósito del Proyecto
* **Proyecto:** SpiroScan AI / VitalSync — Monitor Cardiorrespiratorio IoT con IA.
* **Evento / Nivel:** Feria Tecnológica 2026 (8vo Semestre).
* **Lema / Concepto Central:** *"Un segundo par de oídos para el médico general"*.
* **Audiencia Objetivo:** Comité Mixto (Evaluadores Técnicos + Inversores / Innovación en Salud).
* **Enfoque de la Presentación:** Presentación de Producto en 5 Bloques Estratégicos, basada exclusivamente en evidencia técnica y médica real (cero datos inventados).

---

## 2. Los Dos Niveles de Documentación
1. **Nivel 1 (Documento Maestro de Contenido):**
   * Archivo: `PRESENTACION_PRODUCTO_NIVEL1.md`.
   * Contiene el argumento completo, citas normativas (OMS, NICE, NHLBI, FDA), justificación clínica, evidencia empírica de pruebas en hardware, arquitectura de 4 capas y el desglose financiero completo (BOM, gastos fijos, punto de equilibrio al Mes 8 y corridas a 12 meses).
2. **Nivel 2 (Contenido Sintético para Diapositivas - PENDIENTE / SIGUIENTE PASO):**
   * Archivo a crear: `DIAPOSITIVAS_NIVEL2.md`.
   * Es la versión visual y ejecutiva derivada del Nivel 1, estructurada por diapositivas (Titular de alto impacto, viñetas cortas, cifras clave destacadas, notas del orador e indicaciones de diseño/gráficos).

---

## 3. Estructura de los 5 Bloques Temáticos (Nivel 1)
* **01. Problema:** Subjetividad en auscultación analógica, 1.7 millones de muertes anuales, estetoscopio que atenúa sonidos graves/agudos, inseguridad médica que causa sobrecostos en estudios innecesarios, y vacío de mercado.
* **02. Propuesta:** Vista general en 4 capacidades (captura I2S, memoria en LittleFS, clasificación por IA, triaje determinista) + 4 diferenciadores (hardware abierto, prioridad de síntomas de alarma FDA/NICE, honestidad clínica/SpO2 no inventada, ecosistema App 60 FPS + LLM local).
* **03. Demostración:** Grabación física real de 15 s en hardware ESP32 (`rec_20261006_165553_0f58`), CNN cardíaca auditada (89.7% sens, 91.6% espec, AUC 0.97 en 1,226 audios), sibilancias ICBHI (AUC 0.72) y Banco de Pruebas interactivo en la App móvil.
* **04. Solidez Técnica y Limitaciones:** Arquitectura de 4 capas (ESP32 $\rightarrow$ FastAPI SQLite WAL $\rightarrow$ Inferencia PyTorch/Ollama $\rightarrow$ React Native). Decisiones éticas: por qué se ocultaron crepitantes (AUC 0.53) y soplos filtrados.
* **05. Viabilidad, Costes e Impacto:**
  * BOM unitario: Q1,149.87 (~$147 USD) vs. mercado $400–$600 USD. Venta: Q1,786.00 (margen neto Q546.00).
  * Gastos fijos: Q32,575.00/mes.
  * 4 Planes comerciales (Consultorio, En cuotas, Clínica, Comunitario).
  * Proyección a 12 meses: 195 equipos colocados, Q600,676 ingresos anuales, **Punto de equilibrio en Mes 8 (+Q2,815 netos)** y valle de caja de Q152,183 (Mes 7).
  * Impacto en salud y hoja de ruta en 3 fases.

---

## 4. Próximos Pasos para Continuar en este Repositorio
1. **Generar el Nivel 2 (`DIAPOSITIVAS_NIVEL2.md`):**
   * Sintetizar cada uno de los 5 bloques en una secuencia de 10 a 12 diapositivas.
   * Diseñar la distribución de cada slide: Título $\rightarrow$ Mensaje Clave $\rightarrow$ Datos/Gráfico $\rightarrow$ Notas de orador.
2. **Exportación a Formatos Visuales:**
   * Crear presentación en HTML interactivo (Reveal.js / Marp) o exportar para PowerPoint / Google Slides / Canva.
