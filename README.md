# 🩺 Repositorio de Presentación — SpiroScan AI (VitalSync)

> **Proyecto:** Sistema Embebido para Captura y Análisis de Señales Cardiorrespiratorias  
> **Lema:** *"Un segundo par de oídos para el médico general"*  
> **Audiencia:** Comité Mixto (Evaluadores Técnicos + Inversores / Innovación en Salud)  
> **Repositorio de Origen (Código y Firmware):** `/Users/wilsonjonatan/Documents/8vo 2026/f tecno/FeriaTecnologica2026`

---

## 📂 Archivos en este Directorio

| Archivo | Nivel | Estado | Descripción |
| :--- | :---: | :---: | :--- |
| **[`PRESENTACION_PRODUCTO_NIVEL1.md`](PRESENTACION_PRODUCTO_NIVEL1.md)** | **Nivel 1** | **Completado (100%)** | Documento maestro con todo el contenido, argumentos detallados, citas normativas, justificación clínica, evidencia experimental de hardware y corridas financieras completas. |
| **[`INSTRUCCIONES_PRESENTACION.md`](INSTRUCCIONES_PRESENTACION.md)** | **Metodología** | **Completado (100%)** | Guía metodológica que explica el flujo de trabajo entre Nivel 1 y Nivel 2, los 5 bloques temáticos y las pautas para derivar diapositivas. |
| **[`DIAPOSITIVAS_NIVEL2.md`](DIAPOSITIVAS_NIVEL2.md)** | **Nivel 2** | **En Progreso (11 diapositivas: Problema, Propuesta y Viabilidad)** | Guion y contenido sintético para las diapositivas de la presentación (titulares, viñetas visuales, datos clave y notas de orador). |

---

## 🎯 Estructura de la Presentación (5 Bloques Estratégicos)

1. **01. Problema:**
   * Concepto *"Un segundo par de oídos para el médico general"*.
   * Impacto de 1.7 millones de muertes anuales por afecciones cardiopulmonares (OMS).
   * Limitación del estetoscopio convencional (atenúa graves cardíacos y agudos pulmonares).
   * Inseguridad diagnóstica en atención primaria $\rightarrow$ sobrecostos por estudios innecesarios y derivaciones tardías.
   * Vacío de mercado: estetoscopios de $500 USD vs. gadgets que inventan datos.
   * Citas clínicas breves: OMS, NICE NG115/NG245, NHLBI/AHA, FDA, PhysioNet, CirCor e ICBHI.
2. **02. Propuesta:**
   * Vista general de la solución en 4 capacidades concretas.
   * 4 Diferenciadores de producto: 1. Hardware híbrido abierto (ESP32 + INMP441 I2S + MAX30102 I2C), 2. Triaje determinista FDA/NICE con prioridad en síntomas de alarma, 3. Honestidad clínica radical (SpO2 en espera, sin datos simulados, semáforo gris de incertidumbre), 4. Ecosistema completo (App móvil a 60 FPS con torso interactivo + LLM local).
3. **03. Demostración (Evidencia Experimental):**
   * Grabación física real de 15.0 s (240k muestras a 16 kHz mono en LittleFS, -67.9 a -39.1 dBFS).
   * Reevaluación reproducible de IA cardíaca en 1,226 audios: Sensibilidad 89.70%, Especificidad 91.64%, AUC 0.9708.
   * Detección de sibilancias con ICBHI 2017: AUC ~0.72.
   * Banco de Pruebas ICBHI interactivo en la App móvil para demostración en vivo.
   * Batería de más de 70 pruebas automatizadas aprobadas.
4. **04. Solidez Técnica y Limitaciones Responsables:**
   * Arquitectura de 4 capas desacoplada y offline-first.
   * Decisiones éticas de ingeniería: por qué se ocultaron crepitantes (AUC 0.53) y clasificación multiclase (47%) y por qué se suspendió el descriptor de soplos (fuga de datos previa).
   * Estado físico de sensores y ecualizador acústico por software.
5. **05. Viabilidad, Costes e Impacto:**
   * Costo de fabricación unitario (BOM): **Q1,149.87** (~$147 USD) frente a mercado de $400–$600 USD. Venta: **Q1,786.00** (margen unitario: **Q546.00**).
   * Gastos fijos operativos: **Q32,575.00 / mes** e inversión inicial de **Q34,583.00**.
   * 4 Planes comerciales y punto de equilibrio: Consultorio (138 clientes), En cuotas (138 clientes), Clínica (58 clientes), Comunitario (83 clientes).
   * Proyección financiera a 12 meses: 195 equipos colocados, Q600,676 ingresos anuales, **Punto de equilibrio mensual alcanzado en el Mes 8 (+Q2,815 netos)** y ganancia en Mes 12 de **+Q27,397/mes**.
   * Retorno social en atención primaria y hoja de ruta en 3 fases.

---

## 🛠️ Instrucciones para Continuar Trabajando

### Para crear el Nivel 2 (`DIAPOSITIVAS_NIVEL2.md`):
1. **Regla de oro:** No inventar contenido nuevo; todo debe sintetizarse a partir de `PRESENTACION_PRODUCTO_NIVEL1.md`.
2. **Estructura recomendada para cada diapositiva:**
   ```markdown
   ### Slide X: [Titular de Alto Impacto]
   * **Propósito:** Qué debe entender la audiencia en 5 segundos.
   * **Contenido Visual / Viñetas:** 3 a 4 puntos sintéticos con cifras destacadas en negrita.
   * **Gráfico / Elemento Visual Sugerido:** Mockup, esquema de arquitectura o gráfica financiera.
   * **Notas del Orador:** Guion verbal exacto de 30 a 45 segundos para quien expone.
   ```
3. **Distribución estimada de 10 a 12 slides:**
   * Slide 1: Portada y Lema (*Un segundo par de oídos*).
   * Slide 2: El Problema Epidemiológico y la Auscultación Analógica.
   * Slide 3: Inseguridad Médica y Sobrecostos en el Sistema de Salud.
   * Slide 4: Nuestra Propuesta: Las 4 Capacidades de SpiroScan.
   * Slide 5: Los 4 Diferenciadores de Producto y Ética de Datos.
   * Slide 6: Evidencia en Hardware: Adquisición Física de Audio I2S.
   * Slide 7: Desempeño Auditado de los Modelos de IA.
   * Slide 8: Demostración en Vivo: App Móvil y Banco de Pruebas.
   * Slide 9: Arquitectura de 4 Capas y Transparencia Técnica.
   * Slide 10: Viabilidad Financiera, Costos de Fabricación y Break-even (Mes 8).
   * Slide 11: Impacto en Salud Pública y Hoja de Ruta.
   * Slide 12: Cierre y Preguntas.
