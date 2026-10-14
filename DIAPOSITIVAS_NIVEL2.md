# SpiroScan AI (VitalSync) — Presentación Ejecutiva de Producto
## Guion Maestro de Diapositivas: Puntos 1 y 2 (Problema y Propuesta)

> **Documento Maestro:** [`PRESENTACION_PRODUCTO_NIVEL1.md`](PRESENTACION_PRODUCTO_NIVEL1.md)  
> **Archivo en Vivo:** [`index.html`](index.html#L163) (6 Diapositivas interactivas operativas)  
> **Lema Central:** *"Un segundo par de oídos para el médico general"*  
> **Audiencia:** Comité Mixto (Evaluadores Técnicos + Inversores / Innovación en Salud)  
> **Regla de Integridad:** Cero datos inventados. Todo respaldado documentalmente por la OMS, directrices NICE, NHLBI y FDA.

---

## 🗺️ Mapa de Diapositivas Activas (Secuencia de 6 Diapositivas)

| Bloque | Acto | Diapositiva | Enfoque Estratégico | Duración Sugerida |
| :---: | :---: | :--- | :--- | :---: |
| **01. Problema** | **01** | **Slide 1: Portada y Lema** | Apertura, concepto rector (*Un segundo par de oídos*) y marco de la Feria Tecnológica 2026. | 35 s |
| | **02** | **Slide 2: La Falla de 1816 y 1.7M de Vidas** | Crisis epidemiológica de la OMS y barrera acústica física (graves <200 Hz y agudos >400 Hz). | 40 s |
| | **03** | **Slide 3: Inseguridad y Sobrecostos** | El doble desenlace clínico: sobrecostos por hiper-derivación vs. derivaciones tardías peligrosas. | 40 s |
| | **04** | **Slide 4: El Vacío de Mercado** | El dilema del médico: equipos hospitalarios de $500 USD vs. gadgets fraudulentos $\rightarrow$ SpiroScan AI. | 40 s |
| **02. Propuesta** | **05** | **Slide 5: Las 4 Capacidades Integradas** | Captura digital I2S, almacenamiento flash LittleFS, clasificación IA y triaje determinista con PDF. | 40 s |
| | **06** | **Slide 6: Diferenciadores y Honestidad Clínica** | Hardware abierto ESP32, prioridad vital FDA/NICE, Semáforo Gris (cero inventos) y App 60 FPS + LLM local. | 40 s |

---

# BLOQUE 01: EL PROBLEMA
*(¿Qué necesidad real estamos resolviendo y por qué la tecnología actual falla?)*

---

### Slide 1: Portada y Lema Central
* **Acto / Selector:** Acto 01 de 06 (`data-name="Portada"`).
* **Skin Visual:** `data-skin="problem"` (Fondo azul clínico `#eff4ff`, acento azul profundo `#1d4ed8`).
* **Titular Principal:**
  * **Línea 1:** `SPIROSCAN AI`
  * **Línea 2 (Acento inverso):** `UN SEGUNDO PAR`
  * **Línea 3 (Acento azul):** `DE OÍDOS.`
* **Propósito (5 segundos):** Establecer de inmediato la identidad del producto y el concepto rector: un asistente inteligente de auscultación digital para el médico de primer contacto frente a la saturación de la consulta.

#### Contenido en Pantalla:
* **Bajada:** Asistente biomédico inteligente de auscultación digital para el médico general frente a la saturación de la consulta y la subjetividad del estetoscopio convencional.
* **Badges / Pilares:**
  * `FERIA TECNOLÓGICA 2026`
  * `ATENCIÓN PRIMARIA`
  * `CERO DATOS INVENTADOS`

#### Notas del Orador (35 segundos):
> *"Muy buenos días a los miembros del comité. Presentamos SpiroScan AI: un monitor cardiorrespiratorio inteligente desarrollado bajo una premisa fundamental: ser **un segundo par de oídos para el médico general**.*  
> *La auscultación clínica requiere años de entrenamiento auditivo que, en consultas de atención primaria saturadas, no siempre es posible consolidar. Frente a esa subjetividad, aportamos telemetría digital accesible, rigor clínico y cero datos inventados."*

---

### Slide 2: La Crisis Epidemiológica y la Falla Acústica de 1816
* **Acto / Selector:** Acto 02 de 06 (`data-name="Falla de 1816"`).
* **Skin Visual:** `data-skin="problem"`
* **Titular Principal:**
  * **Línea 1:** `1.7 MILLONES`
  * **Línea 2:** `DE VIDAS.`
  * **Línea 3:** `TUBO DE 1816.`
* **Propósito (5 segundos):** Confrontar la cifra oficial de mortalidad cardiopulmonar evitable con el atraso tecnológico de 210 años del estetoscopio analógico.

#### Contenido en Pantalla (Grid de 2 Columnas):
* **Contexto Izquierdo:** 1.7 millones de personas mueren anualmente por afecciones cardiopulmonares específicas directamente detectables en fases tempranas mediante auscultación y oximetría (OMS).
* **Lista de Limitaciones Físicas (Derecha):**
  * `01` **GRAVES CARDÍACOS (<200 Hz):** Tonos S1/S2 y soplos diastólicos se enmascaran fácilmente con el ruido ambiental de la consulta clínica saturada.
  * `02` **AGUDOS PULMONARES (>400–1000 Hz):** Sibilancias y estertores finos resultan inaudibles si el paciente no respira profundamente.
  * `03` **SIN MEMORIA ACÚSTICA:** *"La primera escucha se pierde en el aire"*. No existe registro objetivo para comparar evolución ni telemedicina.
* **Cierre:** `LIMITACIÓN FÍSICA INSALVABLE`

#### Notas del Orador (40 segundos):
> *"Cada año mueren en el mundo 1.7 millones de personas por patologías directamente detectables con auscultación temprana. Sin embargo, el médico de primer contacto sigue dependiendo de un tubo de goma pasivo inventado en 1816.*  
> *Físicamente, este instrumento atenúa las señales más críticas: los tonos cardíacos graves bajo 200 Hertz se ahogan en el ruido ambiental de la consulta, y las sibilancias pulmonares sobre 400 Hertz son inaudibles con respiraciones superficiales. Y lo más grave: el sonido no se guarda. Si el médico duda, esa primera escucha se pierde para siempre."*

---

### Slide 3: Inseguridad Diagnóstica y Sobrecostos en Salud
* **Acto / Selector:** Acto 03 de 06 (`data-name="Inseguridad y costos"`).
* **Skin Visual:** `data-skin="problem"`
* **Titular Principal:**
  * **Línea 1:** `LA DUDA`
  * **Línea 2 (Acento inverso):** `DIAGNÓSTICA`
  * **Línea 3:** `CUESTA CARO.`
* **Propósito (5 segundos):** Evidenciar el impacto económico y clínico de la incertidumbre en atención primaria, respaldado en directrices internacionales.

#### Contenido en Pantalla (Dos Bloques de Consecuencias):
* **Bajada:** La dificultad del médico de primer contacto para confirmar si un sonido es patológico genera dos desenlaces perjudiciales:
* **Tarjeta 1 (Peligro): Sobrecostos por Hiper-Derivación**
  * Envío masivo de pacientes a radiografías de tórax, ecocardiogramas y tomografías de urgencia simplemente para descartar dudas acústicas básicas, saturando los servicios de salud y encareciendo la atención.
* **Tarjeta 2 (Peligro): Derivaciones Tardías Peligrosas**
  * Pacientes con soplos silentes o broncoespasmos tempranos que regresan a casa sin confirmar y terminan meses después ingresando a urgencias hospitalarias en insuficiencia descompensada.
* **Barra de Cierre:** `REFERENCIAS: NICE NG115/NG245 · NHLBI/AHA` | `INSEGURIDAD MÉDICA`

#### Notas del Orador (40 segundos):
> *"Cuando un médico no especialista tiene dudas sobre lo que acaba de auscultar, se generan dos desenlaces críticos. El primero es el sobrecosto: para descartar una sospecha que no puede confirmar con el oído, envía al paciente a rayos X, tomografías o ecocardiogramas urgentes, saturando los hospitales y encareciendo la atención.*  
> *El segundo desenlace es la derivación tardía: el paciente que se envía a casa con un soplo no detectado y regresa meses después en insuficiencia cardíaca descompensada. La duda diagnóstica no es solo un problema médico; es un drenaje de recursos públicos."*

---

### Slide 4: El Vacío de Mercado y la Respuesta SpiroScan AI
* **Acto / Selector:** Acto 04 de 06 (`data-name="Vacío de mercado"`).
* **Skin Visual:** `data-skin="problem"`
* **Titular Principal:**
  * **Línea 1:** `DOS EXTREMOS`
  * **Línea 2 (Acento inverso):** `INEFICIENTES.`
* **Propósito (5 segundos):** Demostrar la oportunidad comercial y de impacto social que existe entre los equipos de $500 USD y los gadgets fraudulentos.

#### Contenido en Pantalla (Dos Bloques Comparativos):
* **Bajada:** Hoy el médico de atención primaria se encuentra atrapado entre dos opciones inviables:
* **Tarjeta 1: $300 – $600 USD (Estetoscopios Electrónicos Hospitalarios)**
  * Dispositivos comerciales importados (Q2,500–Q5,000) con precios prohibitivos para centros de salud públicos, médicos generales o estudiantes en formación.
* **Tarjeta 2: Fraude Comercial (Gadgets de Consumo Masivo)**
  * Relojes y pulseras de consumo que inventan valores de SpO2, HRV o presiones arteriales no medibles mediante algoritmos generativos sin sensores calibrados.
* **Barra de Cierre:** `LA RESPUESTA: SPIROSCAN AI` | `HARDWARE ABIERTO · RIGOR CLÍNICO`

#### Notas del Orador (40 segundos):
> *"En el mercado actual solo existen dos extremos ineficientes: por un lado, estetoscopios electrónicos importados de 300 a 600 dólares, completamente inaccesibles para la red de atención primaria y puestos de salud comunitarios.*  
> *Por el otro, gadgets de consumo masivo que caen en el fraude tecnológico, inventando valores de signos vitales mediante algoritmos que no miden fisiología real.*  
> *SpiroScan AI rompe esa trampa: un dispositivo biomédico abierto, de bajo costo de fabricación, con sensores digitales de grado médico y honestidad científica absoluta."*

---

# BLOQUE 02: LA PROPUESTA DE VALOR
*(¿Qué hace nuestra solución y por qué es radicalmente diferente?)*

---

### Slide 5: Las 4 Capacidades Integradas de SpiroScan AI
* **Acto / Selector:** Acto 05 de 06 (`data-name="Las 4 capacidades"`).
* **Skin Visual:** `data-skin="prototype"` (Fondo gris técnico `#f4f7fb`, acento azul profundo `#1d4ed8`).
* **Titular Principal:**
  * **Línea 1:** `CUATRO CAPACIDADES.`
  * **Línea 2 (Acento azul):** `UN SOLO SISTEMA.`
* **Propósito (5 segundos):** Presentar la arquitectura funcional de SpiroScan AI organizada en 4 etapas complementarias que acompañan la consulta médica.

#### Contenido en Pantalla (Grid de 4 Módulos):
* **Bajada:** Materializamos el concepto de *"un segundo par de oídos para el médico general"* a través de una arquitectura integrada de tamizaje y telemetría:
* **Módulo `01`: Captura Digital I2S**
  * Aislamiento y realce activo de frecuencias cardíacas graves (<200 Hz) y pulmonares agudas (>400 Hz) sin pérdida analógica del tubo tradicional.
* **Módulo `02`: Memoria Acústica Local**
  * Almacenamiento local en LittleFS. El médico puede pausar, volver a escuchar, medir y contrastar la auscultación sin prisa.
* **Módulo `03`: Clasificación por IA**
  * Redes neuronales convolucionales entrenadas con bases internacionales para detectar sibilancias y patrones acústicos de riesgo.
* **Módulo `04`: Triaje y Reporte PDF**
  * Semáforo clínico protocolizado de prioridad vital y generación automática de informe trazable para referencia médica en la misma consulta.
* **Barra de Cierre:** `SPIROSCAN AI: TAMIZAJE ORIENTATIVO DE BAJO COSTO` | `4 CAPACIDADES EN LA CONSULTA`

#### Notas del Orador (40 segundos):
> *"Para materializar este concepto, SpiroScan AI integra cuatro capacidades esenciales. Primero, captura digital por bus I2S que resalta los componentes graves y agudos sin pérdidas. Segundo, memoria local en memoria flash para que el médico pueda pausar, volver a escuchar y medir sin prisa.*  
> *Tercero, modelos convolucionales de IA que clasifican sibilancias y patrones compatibles con soplos. Y cuarto, un motor de triaje determinista que genera un reporte clínico oficial en PDF en la misma consulta para respaldar la decisión médica."*

---

### Slide 6: Los 4 Diferenciadores y la Honestidad Clínica
* **Acto / Selector:** Acto 06 de 06 (`data-name="Diferenciadores y ética"`).
* **Skin Visual:** `data-skin="prototype"`
* **Titular Principal:**
  * **Línea 1:** `HONESTIDAD CLÍNICA.`
  * **Línea 2 (Acento azul):** `CERO INVENTOS.`
* **Propósito (5 segundos):** Demostrar el rigor técnico y la ética biomédica del proyecto: priorizar síntomas de alarma y rechazar la simulación de datos vitales.

#### Contenido en Pantalla (Grid de 4 Tarjetas):
* **Bajada:** Cuatro diferenciadores irrenunciables que separan a SpiroScan AI de cualquier juguete o producto comercial de caja negra:
* **Tarjeta `01`: Hardware Abierto y Desacoplado**
  * Microcontrolador ESP32 de doble núcleo con micrófono MEMS INMP441 (I2S) y sensor óptico MAX30102 (I2C). Adquisición local confiable y envío seguro por HTTPS sin depender de la nube.
* **Tarjeta `02`: Triaje Determinista (FDA / NICE)**
  * Prioridad vital absoluta: síntomas de alarma (disnea aguda, dolor opresivo, cianosis) activan ROJO inmediato prevaleciendo sobre signos numéricos estables.
* **Tarjeta `03` (Ética Verde): Gestión de Incertidumbre (Semáforo Gris)**
  * Cero datos fabricados: si un sensor no está calibrado físicamente o la señal presenta ruido, el sistema asume la duda y marca datos insuficientes. SpO₂ permanece como no disponible hasta calibración.
* **Tarjeta `04`: Ecosistema App 60 FPS + LLM Local**
  * Torso interactivo en React Native que guía la auscultación en 4 focos cardíacos y pulmonares, banco de pruebas integrado y asistente local LLaMA 3.2 sin filtración de datos de pacientes.
* **Barra de Cierre:** `RESPALDO NORMATIVO: DIRECTRICES FDA · NHLBI · NICE NG115/NG245` | `HONESTIDAD CIENTÍFICA`

#### Notas del Orador (40 segundos):
> *"Nuestra propuesta se distingue por cuatro pilares irrenunciables. El primero es un hardware híbrido abierto con ESP32 de bajo costo. El segundo es un triaje determinista basado en guías FDA y NICE donde los síntomas de alarma tienen prioridad absoluta sobre los números.*  
> *El tercero es honestidad clínica radical: jamás inventamos SpO2 ni signos vitales falsos; si falta calidad, el sistema activa un semáforo gris de datos insuficientes. Y finalmente, un ecosistema completo con app móvil a 60 cuadros por segundo y un modelo de lenguaje local sin filtración de datos a la nube."*

---
*(Fin de los Bloques 01 y 02. Los siguientes bloques 03, 04 y 05 se incorporarán secuencialmente).*
