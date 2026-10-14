# SpiroScan AI (VitalSync) — Presentación de Producto
## Documento Maestro de Contenido para Exposición (Nivel 1)

> **Audiencia Objetivo:** Comité Mixto (Evaluadores Técnicos + Inversores / Innovación en Salud)  
> **Lema / Concepto Central:** *"Un segundo par de oídos para el médico general"*  
> **Propósito:** Base de contenido detallada, argumentada y verificada documental y financieramente, diseñada para derivar posteriormente las diapositivas sintéticas (Nivel 2).  
> **Estructura:** 5 bloques temáticos consolidados (Puntos 5 y 6 unificados en Viabilidad, Costes e Impacto).  
> **Regla de Integridad:** Cero redundancia, datos financieros reales extraídos del estudio de viabilidad (`img_viabilidad/`) y alineación estricta con el alcance técnico verificado del repositorio (`docs/ALCANCE_DEL_PROYECTO.md`, `Backend/knowledge/proyecto.md`, `docs/INFORME_MEJORAS_2026-10-03.md`, `docs/REVISION_ESP32S_2026-10-06.md`, `ENSAYO_FERIA.md`).

---

## 01. Problema — ¿Qué necesidad real estamos resolviendo?

### Mensaje Central y Gancho (The Pitch)
> **"Un segundo par de oídos para el médico general":** Desarrollamos este concepto porque la auscultación clínica requiere años de entrenamiento auditivo y experiencia médica especializada que una persona común —e incluso un médico de primer contacto en una consulta saturada— no siempre puede consolidar. Frente a la subjetividad del estetoscopio convencional, SpiroScan nace como un asistente de auscultación inteligente que ayuda a discernir anomalías acústicas donde el oído humano duda.

### Argumentos Clave en Profundidad
* **Mortalidad cardiopulmonar e impacto epidemiológico:**
  * Alrededor de **1.7 millones de personas mueren anualmente** debido a afecciones cardiopulmonares específicas directamente detectables en etapas tempranas mediante auscultación y oximetría (infecciones respiratorias agudas bajas, crisis asmáticas severas, exacerbaciones de EPOC y cardiopatías valvulares descompensadas).
* **La falla del estetoscopio convencional:**
  * El estetoscopio acústico tradicional (diseñado en 1816) presenta una limitación física insalvable: atenúa frecuencias críticas y no puede amplificar selectivamente los componentes patológicos.
  * No resalta adecuadamente el sonido cardiopulmonar: los sonidos cardíacos graves (tonos S1/S2 y soplos diastólicos <200 Hz) suelen enmascararse con el ruido ambiental de la consulta, mientras que los sonidos pulmonares agudos (sibilancias y estertores finos >400–1000 Hz) pasan desapercibidos si la respiración del paciente es superficial.
* **Inseguridad diagnóstica y sobrecostos en el sistema de salud:**
  * La dificultad para confirmar si un sonido es patológico genera una enorme **inseguridad en el médico no especialista**.
  * Esta incertidumbre desemboca en dos desenlaces perjudiciales:
    1. *Sobrecostos por estudios innecesarios:* Se envían pacientes a radiografías de tórax, ecocardiogramas o tomografías de urgencia simplemente para descartar dudas acústicas básicas, saturando los servicios de salud y encareciendo la atención.
    2. *Derivaciones tardías:* Pacientes con soplos o sibilancias tempranas no son referidos a tiempo por falta de confirmación auditiva, llegando al hospital en fases avanzadas.
* **El vacío del mercado (Los dos extremos ineficientes):**
  * Los estetoscopios electrónicos hospitalarios comerciales existentes tienen precios prohibitivos (**$300 a $600 USD / Q2,500–Q5,000**), inaccesibles para la red de atención primaria o médicos en formación.
  * Los gadgets comerciales de consumo caen en el fraude tecnológico: inventan valores de SpO2, HRV o presión arterial sin calibración fisiológica real.

### Marco Normativo y Fuentes de Referencia
* Cifras epidemiológicas basadas en reportes de la **OMS**; directrices clínicas referenciadas en **NICE NG115/NG245** (respiratorio), **NHLBI/AHA** (cardíaco) y **FDA** (dispositivos acústicos/oximetría). Bases de entrenamiento: **PhysioNet 2016**, **CirCor DigiScope** e **ICBHI 2017**.

### Enlace hacia Nivel 2 (Boceto para Diapositiva)
* *Titular de la Slide:* El Problema: Subjetividad Acústica, Inseguridad Clínica y 1.7 Millones de Vidas en Riesgo.
* *Elementos Visuales:* Concepto "Segundo par de oídos" + Estadística OMS (1.7M) + Cuadro comparativo: Estetoscopio analógico 1816 (atenúa sonido) vs. Incertidumbre médica (estudios innecesarios) vs. Vacío de mercado.

---

## 02. Propuesta — ¿Qué hace nuestra solución y por qué es diferente?

### Mensaje Central
> SpiroScan AI (VitalSync) es una plataforma integral de telemetría y tamizaje biomédico orientativo de bajo costo que fusiona auscultación digital por bus I2S y fotopletismografía I2C, respaldada por un motor de triaje determinista y modelos de IA auditados, bajo un principio irrenunciable: honestidad científica y cero datos fabricados.

### Vista General de la Solución que Ofrecemos
SpiroScan AI materializa el concepto de "un segundo par de oídos para el médico general" a través de 4 capacidades integradas:
1. **Captura y Acondicionamiento Digital:** Sensor digital I2S que resalta y aísla los componentes graves cardíacos (<200 Hz) y agudos pulmonares (>400 Hz) sin las atenuaciones del tubo de goma analógico.
2. **Medición, Repetición y Memoria Acústica:** Almacenamiento local en memoria flash que permite al médico volver a escuchar la auscultación, medirla y reevaluarla sin prisa.
3. **Clasificación Asistida por IA:** Redes convolucionales entrenadas con datos clínicos internacionales para identificar sibilancias y patrones compatibles con soplos.
4. **Triaje Determinista y Reporte Inmediato:** Semáforo orientativo protocolizado que respalda la decisión médica y genera un informe PDF trazable.

### Argumentos Clave en Profundidad (Diferenciadores del Producto)
* **1. Dispositivo de Captura Híbrida y Abierta:**
  * Integra captura acústica torácica digital de alta fidelidad (**micrófono MEMS INMP441 por bus I2S**) y sensor óptico reflexivo (**MAX30102 por bus I2C**) controlados por un microcontrolador de doble núcleo (**ESP32 / NodeMCU-32S**).
  * Arquitectura modular y desacoplada: el dispositivo adquiere de forma confiable, almacena localmente y transmite por HTTPS seguro a un backend central de procesamiento.
* **2. Triaje Determinista con Prioridad Vital de Alarma:**
  * A diferencia de sistemas que usan "IA de caja negra" para diagnosticar enfermedades a ciegas, SpiroScan utiliza un motor de reglas clínicas estrictas (`clinical_assessment.py`) sustentado en directrices **FDA, NHLBI y NICE**.
  * La presencia de síntomas de alarma (disnea aguda, dolor opresivo de pecho, cianosis) activa el semáforo ROJO de inmediato, prevaleciendo sobre signos vitales numéricos aparentemente estables.
* **3. Honestidad Clínica Radical y Gestión de Incertidumbre:**
  * **Cero inventos:** La SpO2 permanece explícitamente como *no disponible* hasta que se valide su calibración física con el circuito real; no se sintetizan HRV ni presiones arteriales no medibles.
  * **Semáforo Gris (Datos Insuficientes):** El sistema asume activamente la incertidumbre. Prefiere indicar que faltan datos antes que emitir un falso verde o un diagnóstico riesgoso.
* **4. Ecosistema de Usuario Completo (Edge + App + LLM Local):**
  * **App Móvil / Web (Expo React Native):** Dispone de un torso anatómico interactivo que guía la auscultación en los 4 focos cardíacos y focos pulmonares, monitor a 60 FPS, banco de pruebas de validación y generación de reportes clínicos oficiales en PDF.
  * **IA Explicativa Aterrizada:** Un modelo de lenguaje local (LLaMA 3.2 3B en Ollama) traduce los hallazgos a lenguaje claro para el paciente o el evaluador, con prompts blindados para evitar alucinaciones médicas.

### Evidencia y Datos Verificados
* **Código de referencia:** [`Backend/clinical_assessment.py`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/Backend/clinical_assessment.py) (reglas de triaje deterministas).
* **Base de conocimiento verificado:** [`Backend/knowledge/proyecto.md`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/Backend/knowledge/proyecto.md).
* **Definición de producto:** Prototipo de tamizaje y telemetría orientativa para referencia médica, no sustituto de diagnóstico médico definitivo.

### Enlace hacia Nivel 2 (Boceto para Diapositiva)
* *Titular de la Slide:* SpiroScan AI: Tamizaje Inteligente, Accesible y Rigurosamente Honesto.
* *Elementos Visuales:* Vista general de 4 capacidades $\rightarrow$ 3 pilares diferenciadores: 1. Hardware abierto I2S/I2C $\rightarrow$ 2. Triaje determinista FDA/NICE $\rightarrow$ 3. Experiencia clínica (App móvil con torso interactivo + PDF).

---

## 03. Demostración — ¿Qué evidencia demuestra que funciona?

### Mensaje Central
> La funcionalidad de SpiroScan no es una maqueta conceptual: está respaldada por capturas físicas de audio digital en hardware real de 15 segundos sin pérdidas, una auditoría reproducible de IA cardíaca sobre 1,226 audios con 89.7% de sensibilidad, y un banco de pruebas clínico interactivo plenamente operativo en la aplicación.

### Argumentos Clave en Profundidad
* **Adquisición física real verificada en hardware ESP32:**
  * Grabación física completa de 15.0 segundos continuos (240,000 muestras PCM a 16 kHz mono, 480 KB) iniciada remotamente desde la interfaz web/móvil (`rec_20261006_165553_0f58`).
  * Almacenamiento local previo en memoria flash con **LittleFS** y transmisión íntegra por **HTTPS** sin pérdidas de paquetes por fluctuaciones de red. Señal digital captada en rango acústico real entre **-67.9 y -39.1 dBFS**, registrada en base de datos con procedencia `real`.
* **Auditoría reproducible del modelo cardíaco (CirCor DigiScope + PhysioNet):**
  * Reevaluación exhaustiva sobre **1,226 grabaciones de audio** con partición estricta por paciente:
    * **Sensibilidad (detección de patológicos):** 89.70% (209 verdaderos positivos vs. 24 falsos negativos).
    * **Especificidad (reconocimiento de sanos):** 91.64% (910 verdaderos negativos vs. 83 falsos positivos).
    * **AUC-ROC:** 0.9708.
  * *Rigor auditado:* Se documenta explícitamente que la especificidad varía según la fuente (ej. PhysioNet-a en ~53.6%), evitando generalizaciones engañosas.
* **Modelo Pulmonar con ICBHI 2017 (Detección de Sibilancias):**
  * Red neuronal convolucional evaluada en pacientes no vistos de la base internacional ICBHI 2017:
    * **Detección de sibilancias (*wheezes*):** Activa en la aplicación con **AUC ~0.72** (detecta ~59% de patologías con sibilancias y reconoce ~81% de ciclos normales).
* **Banco de Pruebas Clínico Integrado en la App:**
  * Permite al jurado, médicos o evaluadores cargar casos clínicos reales precargados (paciente sano, paciente con sibilancias, o sospecha de neumonía) para auditar la respuesta del motor de triaje y la IA en tiempo real sin requerir auscultar a una persona en el estrado.
* **Batería de Calidad y Pruebas de Software:**
  * **Más de 70 pruebas automatizadas aprobadas:** 69 pruebas en Backend (`Backend/tests/` cubriendo flujos clínicos, aislamiento de sesiones y calidad), pruebas C++ de estado óptico/FIFO y verificación TypeScript sin errores.

### Evidencia y Datos Verificados
* **Grabación física de prueba:** `rec_20261006_165553_0f58` (SQLite `telemetry.db`).
* **Auditoría de IA:** [`IA/audit_models.py`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/IA/audit_models.py) y resultados reproducibles en [`IA/docs/audit_results.json`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/IA/docs/audit_results.json).
* **Pruebas de software:** Suite `Backend/tests/` ejecutada con éxito.

### Enlace hacia Nivel 2 (Boceto para Diapositiva)
* *Titular de la Slide:* Evidencia Experimental: Adquisición Física Real y Validación de Modelos.
* *Elementos Visuales:* Gráfico de métricas de IA (Sensibilidad 89.7% / Especificidad 91.6% / AUC 0.97) + Captura de la App con el Banco de Pruebas ICBHI y espectrograma del audio real de 15 s.

---

## 04. Solidez técnica y limitaciones — ¿Cómo está construida y cuáles son sus límites?

### Mensaje Central
> SpiroScan se sustenta en una arquitectura desacoplada de 4 capas sin dependencias cloud obligatorias, cuyo valor diferencial radica en la transparencia técnica: el sistema no solo reporta lo que funciona, sino que oculta o descarta conscientemente aquellos modelos y lecturas que no alcanzan estándares de seguridad clínica.

### Argumentos Clave en Profundidad
* **Arquitectura Robusta de 4 Capas:**
  1. *Capa Embebida (ESP32):* Adquisición I2S e I2C, búfer en LittleFS, stack TLS nativo con verificación de certificado `ISRG Root X1`, reloj NTP y watchdog hardware de 30 s.
  2. *Capa Backend (FastAPI + Mac Studio / Host):* Almacenamiento concurrente en SQLite WAL, colas de audio asíncronas, motor de reglas determinista y renderizado de informes PDF.
  3. *Capa de Inteligencia Artificial:* Inferencia local con PyTorch (CNN espectrogramas Mel) y LLM local (Ollama) sin telemetría externa ni filtración de datos de pacientes.
  4. *Capa de Interfaz (Expo React Native):* Multiplataforma (Web/Móvil), renderizado a 60 FPS con aislamiento de sesión por paciente.
* **Transparencia en Limitaciones y Rechazo de Modelos Poco Confiables:**
  * **Crepitantes (*Crackles*) y Clasificación de Enfermedades Desactivados:** El clasificador de crepitantes obtuvo un AUC de 0.53 (equivalente al azar) y el clasificador multiclase alcanzó un acierto balanceado de solo 47% debido al severo desbalance de la base ICBHI. En lugar de presentarlos como "logros", se ocultaron de la interfaz para proteger la seguridad clínica.
  * **Descriptor de Soplos Desactivado por Contaminación:** Se detectó que el código anterior tenía fuga de datos (*data leakage*, 31 de 36 pacientes de prueba compartidos con el entrenamiento). El módulo fue suspendido preventivamente hasta reentrenar con separación estricta.
* **Estado Físico Actual de Sensores:**
  * *Micrófono INMP441:* Totalmente operativo y validado en hardware.
  * *Sensor Óptico MAX30102:* Firmware listo con rechazo de falsos contactos; a nivel físico presentó NACK en bus I2C (en revisión de cableado/continuidad). El sistema reporta `sensor_unavailable` en lugar de emitir lecturas arbitrarias.
  * *Ecualizador Acústico:* Filtro inverso por software listo en [`Backend/ml/equalizer.py`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/Backend/ml/equalizer.py); se mantiene apagado hasta medir la curva de transferencia física del cabezal con el barrido en fantoma.

### Evidencia y Datos Verificados
* **Reporte de revisión de hardware:** [`docs/REVISION_ESP32S_2026-10-06.md`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/docs/REVISION_ESP32S_2026-10-06.md).
* **Filtros de calidad:** [`Backend/measurement_quality.py`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/Backend/measurement_quality.py).
* **Auditoría de fugas:** [`docs/INFORME_MEJORAS_2026-10-03.md`](file:///Users/wilsonjonatan/Documents/8vo%202026/f%20tecno/FeriaTecnologica2026/docs/INFORME_MEJORAS_2026-10-03.md).

### Enlace hacia Nivel 2 (Boceto para Diapositiva)
* *Titular de la Slide:* Arquitectura de 4 Capas y Gestión Responsable de Limitaciones.
* *Elementos Visuales:* Diagrama de bloques de la arquitectura (ESP32 $\rightarrow$ FastAPI $\rightarrow$ PyTorch/Ollama $\rightarrow$ React Native) + Tabla de "Decisiones Éticas de Ingeniería" (lo que se aprobó vs. lo que se desactivó por rigor).

---

## 05. Viabilidad, Costes e Impacto — ¿Cómo se sostiene, qué valor aporta y cuáles son los siguientes pasos?

### Mensaje Central
> SpiroScan demuestra una viabilidad técnica, operativa y financiera sólida: con un costo de fabricación por equipo de **Q1,149.87** (~$147 USD) —muy inferior a los estetoscopios electrónicos comerciales de $400–$600 USD—, un modelo de suscripción que alcanza su **punto de equilibrio al 8vo mes** con 103 suscriptores, y un impacto social inmediato en el triaje de atención primaria rural y periférica.

### Argumentos Clave en Profundidad

#### A. Estructura Exacta del Costo de Fabricación por Equipo (BOM Unitario)
Basado en el desglose oficial de ingeniería y costos de fabricación (`img_viabilidad/`):

| Componente / Insumo | Costo Unitario (Quetzales) | Función / Especificación |
| :--- | :---: | :--- |
| **ESP32 (NodeMCU-32S)** | Q150.00 | Microcontrolador Dual-Core Xtensa, I2S e I2C nativos |
| **Micrófono MEMS INMP441** | Q90.00 | Captura acústica torácica digital a 16 kHz mono |
| **Sensor óptico (MAX30102)** | Q45.00 | Fotopletismografía y oximetría reflectiva |
| **Barra LED Neopixel WS2812** | Q50.00 | Semáforo visual de triaje integrado en el dispositivo |
| **Batería 18650 Li-Ion + Portapilas** | Q69.00 | Alimentación autónoma recargable de 3.7V |
| **Cargador TP4056 + Elevador MT3608** | Q34.00 | Gestión de carga segura y estabilización de voltaje |
| **Cables, estaño y varios de ensamble** | Q50.00 | Conexionado interno |
| **Resistencias, termocontráctil y pegamento**| Q5.74 | Aislamiento y protección pasiva |
| **Filamento PLA (41 g) + TPU (25 g)** | Q14.28 | Carcasa ergonómica impresa en 3D con sello acústico |
| **Empaque + GARANTÍA industrial** | Q615.00 | Presentación clínica y garantía de reemplazo |
| **Luz de impresión 3D y armado (4 h)** | Q1.45 | Costo energético de manufactura aditiva |
| **Reserva de garantía (5% de piezas)** | Q25.40 | Fondo de contingencia por fallas de hardware |
| **TOTAL COSTO DE FABRICAR UN EQUIPO** | **Q1,149.87** | **Aprox. $147 USD (Frente a $400–$600 USD de mercado)** |

* **Precio de venta sin IVA:** **Q1,786.00** (incluye costo, 4 horas de armado técnico y margen).
* **Ganancia neta directa por equipo vendido (una vez):** **Q546.00** (descontando IVA, ISR y costo directo).

---

#### B. Estructura Operativa y Gastos Fijos Mensuales
* **Sueldos del equipo técnico y clínico:** Q29,911.00 / mes (incluye salario base + prestaciones de ley + bonificación para el equipo de desarrollo y soporte).
* **Servidor e infraestructura (amortizado a 3 años):** Q760.00 / mes.
* **Asesoría contable y legal:** Q1,500.00 / mes.
* **Servicios (Internet, electricidad y depreciación):** Q404.00 / mes.
* **TOTAL GASTOS FIJOS OPERATIVOS AL MES:** **Q32,575.00**
* **Inversión inicial requerida (Capital semilla):** **Q34,583.00** (cubre servidor local host, constitución de empresa, lote inicial de 5 equipos y prototipo validado).

---

#### C. Planes Comerciales y Punto de Equilibrio (*Break-even*)
Para adaptarse a distintos niveles de adopción en el sector salud, se establecieron 4 modalidades de comercialización:

| Plan Comercial | Pago Inicial | Mensualidad (Año 1) | Mensualidad (Después) | Ingreso Neto / Mes | Clientes para Punto de Equilibrio |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **1. Consultorio (Compra directa)** | Q2,000.00 | Q280.00 | Q280.00 | Q238.00 | **138 clientes** |
| **2. En cuotas (12 meses, +10%)** | Q0.00 | Q463.00 | Q280.00 | Q238.00 | **138 clientes** |
| **3. Clínica (Paquete 3 equipos, -10%)**| Q5,399.00 | Q672.00 | Q672.00 | Q570.00 | **58 clientes** |
| **4. Comunitario / ONG (Alquiler)** | Q0.00 | Q504.00 | Q504.00 | Q396.00 | **83 clientes** |

---

#### D. Proyección Financiera a 12 Meses y Sostenibilidad
De acuerdo con la corrida financiera proyectada:

* **Evolución de ventas y tracción:**
  * Mes 1: 5 equipos vendidos $\rightarrow$ Mes 4: 12 equipos (35 suscriptores acumulados).
  * Mes 8: 20 equipos vendidos (103 suscriptores acumulados).
  * Mes 12: 25 equipos vendidos (**195 equipos y suscriptores activos en el Año 1**).
* **Ingresos y Rentabilidad:**
  * **Ingresos brutos anuales (sin IVA):** **Q600,676.00**
  * Costo anual de fabricación: Q224,225.00 | Gastos fijos anuales: Q390,899.00 | ISR anual: Q30,034.00
* **Hitos Financieros Críticos:**
  * **Punto de Equilibrio Mensual alcanzado en el Mes 8:** Con 103 suscriptores activos, el flujo mensual pasa a terreno positivo con **+Q2,815.00** de ganancia neta.
  * **Ganancia neta mensual al Mes 12:** **+Q27,397.00 / mes**.
  * **Valle de caja máximo (Capital de trabajo necesario antes del break-even):** **Q152,183.00** (alcanzado en el Mes 7, recuperándose sostenidamente a partir del Mes 8).

---

#### E. Impacto Clínico, Social y Hoja de Ruta (Next Steps)
* **Descongestión de Urgencias y Respaldo al Médico Rural:**
  * Permite al médico general en puestos de salud periféricos auscultar con certeza, comparar el audio contra patrones patológicos y decidir con evidencia técnica a quién referir al hospital, ahorrando traslados innecesarios a familias vulnerables.
* **Hoja de Ruta hacia la Adopción en Campo (3 Fases):**
  * **Fase 1 (Completada - Feria Tecnológica 2026):** Prototipo funcional validado, captura física I2S verificada en hardware, modelos de IA auditados y app con banco de pruebas.
  * **Fase 2 (Inmediata - Corto Plazo):** Corrección física del conexionado I2C del sensor óptico, calibración experimental de SpO2 contra oxímetro clínico de referencia y barrido acústico en fantoma.
  * **Fase 3 (Mediano Plazo - Despliegue Piloto):** Ensayo clínico piloto en centros de salud rurales para validar usabilidad, concordancia diagnóstica y reducción de costos en estudios complementarios.

### Enlace hacia Nivel 2 (Boceto para Diapositiva)
* *Titular de la Slide:* Viabilidad Económica, Punto de Equilibrio y Retorno Social.
* *Elementos Visuales:*
  * Gráfico 1: Desglose de costos (Fabricación Q1,149 vs. Venta Q1,786 vs. Mercado internacional Q3,500+).
  * Gráfico 2: Curva de flujo de caja de 12 meses mostrando el Punto de Equilibrio en el Mes 8 (+Q2,815) y el valle de capital de Q152,183.
  * Gráfico 3: Hoja de ruta en 3 fases hacia el despliegue clínico.
