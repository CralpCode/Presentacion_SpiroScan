# SpiroScan AI (VitalSync) — Presentación Ejecutiva de Producto
## Guion Maestro de Diapositivas: Problema, Propuesta y Viabilidad (11 Diapositivas)

> **Documento Maestro:** [`PRESENTACION_PRODUCTO_NIVEL1.md`](PRESENTACION_PRODUCTO_NIVEL1.md)  
> **Archivo en Vivo:** [`index.html`](index.html#L163) (11 Diapositivas interactivas operativas, optimizadas para 100vh sin scroll vertical)  
> **Lema Central:** *"Un segundo par de oídos para el médico general"*  
> **Audiencia:** Comité Mixto (Evaluadores Técnicos + Inversores / Innovación en Salud)  
> **Regla de Integridad:** Cero datos inventados. Todo respaldado por citas oficiales (OMS, NICE, NHLBI, FDA), costos de ingeniería (BOM Q1,149.87) y corridas financieras a 12 meses.

---

## 🗺️ Mapa de la Presentación (11 Diapositivas Activas)

| Bloque | Acto | Diapositiva | Enfoque Estratégico | Duración |
| :---: | :---: | :--- | :--- | :---: |
| **01. Problema** | **01** | **Slide 1: Portada y Lema** | Apertura, concepto rector (*Un segundo par de oídos*) y marco de la Feria Tecnológica 2026. | 35 s |
| | **02** | **Slide 2: La Falla de 1816 y 1.7M de Vidas** | Crisis epidemiológica de la OMS y barrera acústica física (graves <200 Hz y agudos >400 Hz). | 40 s |
| | **03** | **Slide 3: Inseguridad y Sobrecostos** | El doble desenlace clínico: sobrecostos por hiper-derivación vs. derivaciones tardías peligrosas. | 40 s |
| | **04** | **Slide 4: El Vacío de Mercado** | El dilema del médico: equipos hospitalarios de $500 USD vs. gadgets fraudulentos $\rightarrow$ SpiroScan AI. | 40 s |
| **02. Propuesta** | **05** | **Slide 5: Las 4 Capacidades Integradas** | Captura digital I2S, almacenamiento flash LittleFS, clasificación IA y triaje determinista con PDF. | 40 s |
| | **06** | **Slide 6: Hardware y Ecosistema** | Hardware abierto ESP32 + INMP441 + MAX30102, app a 60 FPS con torso interactivo y LLM local. | 40 s |
| | **07** | **Slide 7: Rigor Clínico y Ética de Datos** | Triaje determinista con prioridad vital FDA/NICE y Semáforo Gris de incertidumbre (cero inventos). | 40 s |
| **05. Viabilidad** | **08** | **Slide 8: Costo Unitario BOM (Q1,149.87)** | Desglose oficial de manufactura vs. mercado internacional ($400–$600 USD) y ganancia neta (Q546). | 45 s |
| | **09** | **Slide 9: Modelo de 4 Planes Comerciales** | Estrategia de adopción: Consultorio, Cuotas (Q0 hoy), Clínica y Comunitario (Alquiler). | 45 s |
| | **10** | **Slide 10: Break-Even y Proyección a 12 Meses** | Punto de equilibrio alcanzado en el Mes 8 (103 suscriptores, +Q2,815) y tracción al Mes 12. | 45 s |
| | **11** | **Slide 11: Retorno Social y Hoja de Ruta** | Impacto en salud pública rural y despliegue en 3 fases (laboratorio $\rightarrow$ calibración $\rightarrow$ piloto). | 40 s |

---

# BLOQUE 01: EL PROBLEMA
*(¿Qué necesidad real estamos resolviendo y por qué la tecnología actual falla?)*

---

### Slide 1: Portada y Lema Central
* **Acto / Selector:** Acto 01 de 11 (`data-name="Portada"`).
* **Skin Visual:** `data-skin="problem"` (Fondo azul clínico `#eff4ff`, acento azul profundo `#1d4ed8`).
* **Titular Principal:** `SPIROSCAN AI` / `UN SEGUNDO PAR` / `DE OÍDOS.`
* **Propósito (5 s):** Establecer de inmediato la identidad del producto y el concepto rector para el médico de primer contacto frente a la saturación de la consulta.
* **Contenido en Pantalla:**
  * Asistente biomédico inteligente de auscultación digital para el médico general frente a la saturación de la consulta y la subjetividad del estetoscopio convencional.
  * Pilares: `FERIA TECNOLÓGICA 2026` · `ATENCIÓN PRIMARIA` · `CERO DATOS INVENTADOS`.
* **Notas del Orador (35 s):**
  > *"Muy buenos días a los miembros del comité. Presentamos SpiroScan AI: un monitor cardiorrespiratorio inteligente desarrollado bajo una premisa fundamental: ser un segundo par de oídos para el médico general. La auscultación clínica requiere años de entrenamiento auditivo que en consultas saturadas no siempre es posible consolidar. Frente a esa subjetividad, aportamos telemetría digital accesible y cero datos inventados."*

---

### Slide 2: La Falla Física de 1816 y los 1.7 Millones de Muertes
* **Acto / Selector:** Acto 02 de 11 (`data-name="Falla de 1816"`).
* **Skin Visual:** `data-skin="problem"`
* **Titular Principal:** `1.7 MILLONES` / `DE VIDAS.` / `TUBO DE 1816.`
* **Propósito (5 s):** Confrontar la cifra oficial de mortalidad evitable con el atraso tecnológico de 210 años del estetoscopio analógico.
* **Contenido en Pantalla (Grid 2 Columnas):**
  * Mortalidad anual de 1.7 millones de personas por afecciones cardiopulmonares detectables tempranamente (OMS).
  * `01` **Graves Cardíacos (<200 Hz):** Tonos S1/S2 y soplos enmascarados por ruido ambiente en la consulta.
  * `02` **Agudos Pulmonares (>400–1000 Hz):** Sibilancias y estertores inaudibles con respiración superficial.
  * `03` **Sin Memoria Acústica:** *"La primera escucha se pierde en el aire"*. Sin registro para comparar evolución ni telemedicina.
* **Notas del Orador (40 s):**
  > *"Cada año mueren en el mundo 1.7 millones de personas por patologías directamente detectables con auscultación temprana. Sin embargo, seguimos dependiendo de un tubo de goma pasivo inventado en 1816 que atenúa físicamente los graves cardíacos bajo 200 Hz y los agudos pulmonares sobre 400 Hz. Además, no guarda audio: la primera escucha se pierde en el aire."*

---

### Slide 3: Inseguridad Diagnóstica y Sobrecostos en Salud
* **Acto / Selector:** Acto 03 de 11 (`data-name="Inseguridad y costos"`).
* **Skin Visual:** `data-skin="problem"`
* **Titular Principal:** `LA DUDA DIAGNÓSTICA` / `CUESTA CARO.`
* **Propósito (5 s):** Demostrar cómo la incertidumbre clínica drena recursos públicos y satura la red hospitalaria.
* **Contenido en Pantalla (2 Tarjetas de Peligro):**
  * **Consecuencia 01: Sobrecostos por Hiper-Derivación:** Envío a rayos X, TAC y ecocardiogramas urgentes para descartar sospechas básicas, saturando hospitales y encareciendo la salud.
  * **Consecuencia 02: Derivaciones Tardías Peligrosas:** Pacientes con soplos o crisis iniciales que regresan a casa sin confirmar y terminan meses después en urgencias hospitalarias descompensados.
  * Citas: `NICE NG115/NG245` · `NHLBI/AHA`.
* **Notas del Orador (40 s):**
  > *"Cuando el médico no especialista duda, ocurren dos tragedias. La primera es el sobrecosto: se ordenan rayos X, TACs o ecocardiogramas urgentes solo para descartar dudas acústicas básicas, saturando hospitales. La segunda es la derivación tardía: el paciente que se va a casa con un soplo no detectado y regresa meses después descompensado a cuidados intensivos."*

---

### Slide 4: El Vacío de Mercado y la Respuesta SpiroScan AI
* **Acto / Selector:** Acto 04 de 11 (`data-name="Vacío de mercado"`).
* **Skin Visual:** `data-skin="problem"`
* **Titular Principal:** `DOS EXTREMOS` / `INEFICIENTES.`
* **Propósito (5 s):** Evidenciar el espacio de mercado desatendido entre equipos inaccesibles y juguetes comerciales.
* **Contenido en Pantalla (2 Tarjetas de Mercado):**
  * **$300 – $600 USD (Estetoscopios Electrónicos Hospitalarios):** Equipos comerciales importados (Q2,500–Q5,000) prohibitivos para centros de salud y médicos generales.
  * **Fraude Comercial (Gadgets de Consumo Masivo):** Relojes y pulseras que inventan SpO2, HRV o presiones con algoritmos sin sensores calibrados.
  * Cierre: `LA RESPUESTA: SPIROSCAN AI` | `HARDWARE ABIERTO · RIGOR CLÍNICO`.
* **Notas del Orador (40 s):**
  > *"En el mercado actual solo existen dos extremos ineficientes: estetoscopios electrónicos extranjeros de 300 a 600 dólares, inaccesibles para la red de atención primaria; o gadgets de pulsera que inventan signos vitales simulados. SpiroScan AI llena este vacío: hardware digital I2S accesible, fabricación local y honestidad clínica verificable."*

---

# BLOQUE 02: LA PROPUESTA DE VALOR
*(¿Qué hace nuestra solución y por qué es radicalmente diferente?)*

---

### Slide 5: Las 4 Capacidades Integradas
* **Acto / Selector:** Acto 05 de 11 (`data-name="Las 4 capacidades"`).
* **Skin Visual:** `data-skin="prototype"` (Fondo gris técnico `#f4f7fb`, acento azul rey `#1d4ed8`).
* **Titular Principal:** `CUATRO CAPACIDADES.` / `UN SOLO SISTEMA.`
* **Propósito (5 s):** Explicar de forma modular cómo SpiroScan AI materializa *"un segundo par de oídos para el médico general"*.
* **Contenido en Pantalla (Grid de 4 Módulos):**
  * `01` **Captura Digital I2S:** Aislamiento y realce activo de graves (<200 Hz) y agudos (>400 Hz) sin pérdidas.
  * `02` **Memoria Acústica:** Almacenamiento local en LittleFS para pausar, repetir, medir y contrastar el audio sin prisa.
  * `03` **Clasificación por IA:** Redes convolucionales entrenadas internacionalmente para sibilancias y patrones compatibles con soplos.
  * `04` **Triaje y Reporte PDF:** Semáforo de prioridad vital protocolizado y generación automática de informe trazable en la consulta.
* **Notas del Orador (40 s):**
  > *"Para materializar este concepto, SpiroScan AI integra cuatro capacidades esenciales. Primero, captura digital por bus I2S que resalta los graves y agudos sin pérdidas. Segundo, memoria local en LittleFS para que el médico pueda pausar, volver a escuchar y medir sin prisa. Tercero, modelos convolucionales de IA que clasifican sibilancias y patrones compatibles con soplos. Y cuarto, un motor de triaje determinista que genera un reporte clínico oficial en PDF en la misma consulta."*

---

### Slide 6: Hardware Abierto y Ecosistema Edge
* **Acto / Selector:** Acto 06 de 11 (`data-name="Hardware y ecosistema"`).
* **Skin Visual:** `data-skin="prototype"`
* **Titular Principal:** `HARDWARE ABIERTO.` / `ECOSISTEMA EDGE.`
* **Propósito (5 s):** Mostrar la solidez de la arquitectura embebida y la experiencia de usuario a 60 FPS sin dependencia de la nube.
* **Contenido en Pantalla (2 Tarjetas de Arquitectura):**
  * `01` **Hardware Híbrido Abierto:** ESP32 Dual-Core con micrófono MEMS INMP441 (I2S) y sensor óptico MAX30102 (I2C). Búfer local en LittleFS y transmisión HTTPS segura.
  * `02` **App 60 FPS + Asistente Local:** Torso anatómico interactivo en React Native que guía los 4 focos cardíacos y pulmonares, con modelo LLaMA 3.2 local (Ollama) para explicar hallazgos sin filtrar datos a la nube.
* **Notas del Orador (40 s):**
  > *"A nivel de ingeniería, combinamos hardware abierto con un microcontrolador ESP32 de doble núcleo y sensores I2S e I2C de bajo costo. Esto se conecta a una aplicación móvil a 60 cuadros por segundo con un torso interactivo de auscultación guiada y un modelo de lenguaje local LLaMA 3.2 que explica los hallazgos en la clínica sin enviar datos de pacientes a servidores en la nube."*

---

### Slide 7: Rigor Clínico y Ética de Datos
* **Acto / Selector:** Acto 07 de 11 (`data-name="Rigor clínico y ética"`).
* **Skin Visual:** `data-skin="lung"` (Fondo celeste clínico `#edf8fc`, acento `#0369a1`).
* **Titular Principal:** `HONESTIDAD CLÍNICA.` / `CERO INVENTOS.`
* **Propósito (5 s):** Demostrar el compromiso ético y normativo que prioriza la seguridad del paciente sobre promesas comerciales infundadas.
* **Contenido en Pantalla (2 Tarjetas de Ética Médica):**
  * `01` **Triaje Determinista (FDA / NICE):** Reglas clínicas estrictas donde los síntomas de alarma (disnea aguda, dolor opresivo, cianosis) activan ROJO inmediato sobre cualquier signo numérico estable.
  * `02` **Semáforo Gris (Incertidumbre Asumida):** Si un sensor no está calibrado físicamente o la señal presenta ruido, el sistema marca "Datos Insuficientes". SpO₂ permanece como no disponible hasta validación real.
* **Notas del Orador (40 s):**
  > *"Nuestra ética biomédica se sustenta en directrices de la FDA y NICE. El triaje es determinista: si un paciente tiene disnea aguda o dolor opresivo de pecho, el semáforo activa ROJO inmediato sin importar si los números parecen estables. Además, gestionamos la incertidumbre con honestidad radical: si un sensor no está calibrado, marcamos datos insuficientes; jamás inventamos SpO2 ni signos vitales falsos."*

---

# BLOQUE 05: VIABILIDAD, COSTES E IMPACTO
*(¿Cómo se sostiene, qué valor aporta y cuáles son los siguientes pasos?)*

---

### Slide 8: Estructura de Costo Unitario (BOM)
* **Acto / Selector:** Acto 08 de 11 (`data-name="Costo unitario BOM"`).
* **Skin Visual:** `data-skin="mint"` (Fondo verde menta `#e9f7ef`, acento `#047857`).
* **Titular Principal:** `FABRICARLO CUESTA` / `Q1,149.87 / EQUIPO.`
* **Propósito (5 s):** Demostrar la viabilidad industrial del dispositivo con el desglose auditado del BOM frente al mercado internacional.
* **Contenido en Pantalla (Grid de 3 Métricas):**
  * `Q1,149.87` **Costo Unitario de Fabricación:** ESP32 (Q150) + INMP441 (Q90) + MAX30102 (Q45) + WS2812 (Q50) + Batería y cargador (Q103) + Carcasa 3D PLA/TPU (Q14.28) + Empaque y garantía industrial (Q615) + Ensamble.
  * `Q1,786.00` **Precio de Venta (Sin IVA):** Cubre costo directo, 4 horas de ensamble técnico calificado y margen operativo.
  * `Q546.00` **Ganancia Neta / Equipo:** Utilidad líquida unitaria descontando costo de manufactura, IVA e impuesto sobre la renta (ISR).
* **Notas del Orador (45 s):**
  > *"Pasando a la viabilidad económica, el costo de fabricar un equipo SpiroScan AI es de exactamente Q1,149.87, equivalente a unos 147 dólares. Esto incluye el microcontrolador, los sensores, la batería recargable, la carcasa aditiva y un fondo de garantía industrial. Frente a los estetoscopios importados de 400 a 600 dólares, nuestro precio de venta de Q1,786 genera un ahorro superior al 55% y un margen neto directo de Q546 por equipo."*

---

### Slide 9: Modelo de 4 Planes Comerciales
* **Acto / Selector:** Acto 09 de 11 (`data-name="Planes comerciales"`).
* **Skin Visual:** `data-skin="pricing"` (Fondo ámbar `#fff9ed`, acento `#a45c08`).
* **Titular Principal:** `CUATRO PLANES.` / `ACCESO FLEXIBLE.`
* **Propósito (5 s):** Presentar la estrategia comercial para acelerar la adopción en consultorios, clínicas y puestos de salud comunitarios.
* **Contenido en Pantalla (Grid 2x2):**
  * `01. CONSULTORIO (Compra directa):` **Q2,000 inicial** + **Q280 / mes**. Propiedad del equipo + plataforma activa. (Punto equilibrio: 138 clientes).
  * `02. EN CUOTAS (12 meses):` **Q0 inicial** + **Q463 / mes × 12** (luego Q280/mes). Sin desembolso inicial. (Equilibrio: 138 clientes).
  * `03. CLÍNICA (3 equipos, -10%):` **Q5,399 inicial** + **Q672 / mes**. Paquete para centros con múltiples médicos. (Equilibrio: 58 clientes).
  * `04. COMUNITARIO / ONG (Alquiler):` **Q0 inicial** + **Q504 / mes**. Gasto operativo puro para brigadas rurales. (Equilibrio: 83 clientes).
  * Cierre: `ACLARACIÓN CLAVE: Q0 HOY NO SIGNIFICA GRATIS` | `MODELO SOSTENIBLE`.
* **Notas del Orador (45 s):**
  > *"Para acelerar la adopción diseñamos cuatro planes comerciales. El plan Consultorio con compra directa de Q2,000; el plan en 12 cuotas con Q0 de pago inicial y mensualidades de Q463; el plan Clínica de 3 equipos por Q5,399; y el plan Comunitario en alquiler puro por Q504 al mes para brigadas u ONGs. Q0 inicial permite que un médico comience de inmediato sin barreras de capital, manteniendo el modelo plenamente autosostenible."*

---

### Slide 10: Punto de Equilibrio y Proyección a 12 Meses
* **Acto / Selector:** Acto 10 de 11 (`data-name="Punto de equilibrio"`).
* **Skin Visual:** `data-skin="growth"` (Modo oscuro `#071827`, acento menta `#76dfba`).
* **Titular Principal:** `PUNTO DE EQUILIBRIO.` / `ALCANZADO EN EL MES 8.`
* **Propósito (5 s):** Probar la sostenibilidad financiera del modelo con gastos fijos operativos de **Q32,575 / mes** y capital semilla de **Q34,583**.
* **Contenido en Pantalla (Grid de 4 Métricas de Tracción):**
  * `MES 8` **Punto de Equilibrio Mensual:** Con **103 suscriptores activos**, el flujo operativo pasa a terreno positivo con **+Q2,815.00** netos al mes.
  * `MES 12` **Rentabilidad Consolidada:** **195 equipos activos** colocados generan una ganancia neta mensual de **+Q27,397.00 / mes**.
  * `Q152,183` **Valle de Caja Máximo:** Capital de trabajo acumulado requerido en el Mes 7 antes de que el flujo se vuelva positivo permanentemente.
  * `Q600,676` **Ingresos Brutos Año 1:** Facturación anual proyectada (sin IVA) cubriendo Q224,225 de producción y Q390,899 de gastos fijos.
* **Notas del Orador (45 s):**
  > *"Nuestra corrida financiera a 12 meses contempla gastos fijos operativos de Q32,575 mensuales. El hito crítico se alcanza en el Mes 8 con 103 suscriptores activos, momento en que el flujo pasa a terreno positivo con +Q2,815 netos mensuales, escalando a +Q27,397 al Mes 12 con 195 equipos colocados y más de Q600,000 en facturación anual. El capital de trabajo necesario antes del break-even es un valle de caja de Q152,183 en el Mes 7."*

---

### Slide 11: Retorno Social y Hoja de Ruta en 3 Fases
* **Acto / Selector:** Acto 11 de 11 (`data-name="Impacto y hoja de ruta"`).
* **Skin Visual:** `data-skin="mint"` (Fondo verde menta `#e9f7ef`, acento `#047857`).
* **Titular Principal:** `RETORNO SOCIAL.` / `HOJA DE RUTA EN 3 FASES.`
* **Propósito (5 s):** Cerrar la presentación conectando la viabilidad comercial con el impacto transformador en la salud pública rural.
* **Contenido en Pantalla (3 Fases Secuenciales):**
  * **Fase 1 (Completada · Feria 2026):** Prototipo funcional validado, captura física I2S en hardware real de 15 s, modelos de IA auditados (89.7% sens) y app con banco de pruebas.
  * **Fase 2 (Inmediata · Corto Plazo):** Corrección física de continuidad I2C en sensor óptico, calibración de SpO2 contra oxímetro de grado clínico y ecualización en fantoma.
  * **Fase 3 (Mediano Plazo · Despliegue Piloto):** Ensayo piloto en puestos de salud comunitarios para validar descongestión de urgencias y reducción de sobrecostos hospitalarios.
  * Cierre: `SPIROSCAN AI (VITALSYNC) · FERIA TECNOLÓGICA 2026` | `UN SEGUNDO PAR DE OÍDOS`.
* **Notas del Orador (40 s):**
  > *"El verdadero valor de SpiroScan AI es su retorno social en salud pública: apoyar al médico general en puestos de salud rurales para descongestionar hospitales y salvar vidas. Nuestra hoja de ruta tiene la Fase 1 validada en laboratorio, la Fase 2 inmediata de calibración óptica en fantoma, y la Fase 3 de despliegue piloto en centros comunitarios. SpiroScan es un segundo par de oídos donde más se necesita."*

---
*(Fin del guion maestro activo de 11 diapositivas).*
