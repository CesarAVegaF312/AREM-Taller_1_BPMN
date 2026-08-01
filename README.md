# 🛠️ Taller 1: Modelado de Proceso del Cliente con BPMN

## 🎯 Objetivo

Modelar un proceso de negocio real del cliente utilizando la notación BPMN, identificando eventos, actividades, decisiones, actores involucrados y puntos críticos del flujo.

---

## 📘 Guía paso a paso

Antes de empezar a modelar, revise la [**Guía Paso a Paso: Cómo Modelar un Proceso en BPMN**](clase/guia_paso_a_paso_bpmn.md). Incluye la leyenda de notación, la metodología de 5 pasos que se usa en todo el taller, un ejemplo completo construido paso a paso sobre el propio caso de la Clínica Salud Viva, y una comparación de errores comunes vs. modelo corregido.

## 🏥 Caso base de referencia: Clínica Salud Viva

Durante este taller, todos los equipos trabajarán en clase con un caso base común antes de aplicarlo a su cliente real.

## 🧠 Contexto

La Clínica Salud Viva es una institución médica de tamaño medio ubicada en una ciudad capital. Atiende pacientes tanto de manera presencial como virtual, y cuenta con una plataforma digital donde los usuarios pueden agendar citas médicas, recibir notificaciones y consultar su historial de atención. El proceso de agendamiento implica la selección de especialidad, disponibilidad del médico y confirmación vía correo electrónico o mensaje de texto. Este proceso es fundamental para garantizar una atención eficiente y organizada, especialmente en épocas de alta demanda como campañas de vacunación o jornadas preventivas.

**Descripción del caso:**
- La Clínica Salud Viva es una clínica mediana que ofrece atención médica presencial y virtual.
- Cuenta con un sistema de gestión de citas en línea, un ERP administrativo y alianzas con aseguradoras de salud.

**Proceso a modelar (en clase):**
> Agendamiento de Citas Médicas

- Actor: Paciente
- Flujo: Selección de especialidad → Médico → Fecha → Confirmación
- Interacciones: con sistema de citas, base de datos, notificación por correo/SMS

---

## 🧪 Parte 1: Trabajo en Clase

Durante la clase se espera que el equipo:

Siga la metodología de 5 pasos de la [guía paso a paso](clase/guia_paso_a_paso_bpmn.md) para modelar el proceso de agendamiento de citas de la Clínica Salud Viva:

1. Identifique los actores del proceso (¿quién participa? ¿qué rol cumple cada uno?).
2. Defina el evento de inicio y los posibles eventos de fin.
3. Liste las actividades principales de cada actor.
4. Inserte los gateways (decisiones) y formule su pregunta.
5. Conecte todo con flujos de secuencia, etiquete las salidas de cada gateway y valide el modelo con la [checklist de autoevaluación](clase/guia_paso_a_paso_bpmn.md#5-checklist-de-autoevaluación-antes-de-entregar).

- Use papel, pizarra o herramientas como draw.io o Camunda Modeler.
- Reciba retroalimentación del docente y registre avances en `clase/notas.md` (use la [plantilla de notas](plantillas/plantilla_notas.md)).

---

## 🧠 Parte 2: Aplicación al Cliente Real

Después de la clase, el equipo debe:

- Seleccionar un proceso real del cliente asignado (puede ser análogo al caso de clase, pero **no puede ser el mismo proceso de agendamiento de citas** — debe corresponder al negocio del cliente).
- Aplicar los mismos 5 pasos de la guía metodológica a ese proceso.
- Digitalizar el modelo BPMN específico del cliente en `entrega/modelo-final.drawio`.
- Redactar el informe en `entrega/informe.md` usando la [plantilla de informe del taller](plantillas/plantilla_informe_taller.md); explicar el proceso, las diferencias con el caso base y las justificaciones de cada decisión de modelado.
- Complementar con una investigación sobre buenas prácticas BPMN y ejemplos en la industria, y registrar las fuentes en `entrega/referencias.md` con la [plantilla de referencias](plantillas/plantilla_referencias.md).

---

## 📁 Estructura esperada del repositorio

```
taller-01-bpmn/
├── README.md
├── clase/
│   ├── guia_paso_a_paso_bpmn.md   # Notación, metodología de 5 pasos y ejemplo guiado
│   ├── img/                       # Diagramas de apoyo de la guía
│   ├── modelo.drawio              # Modelo BPMN del caso base (Clínica Salud Viva)
│   └── notas.md                   # Ver plantillas/plantilla_notas.md
├── entrega/
│   ├── modelo-final.drawio        # Modelo BPMN del proceso real del cliente
│   ├── informe.md                 # Ver plantillas/plantilla_informe_taller.md
│   └── referencias.md             # Ver plantillas/plantilla_referencias.md
└── plantillas/
    ├── plantilla_informe_taller.md
    ├── plantilla_notas.md
    └── plantilla_referencias.md
```

---

## ⚠️ Errores comunes

Antes de entregar, compare su modelo contra los errores más frecuentes (evento de fin faltante, gateways sin pregunta, actividades sin conectar, carriles ausentes) documentados en la [sección 4 de la guía paso a paso](clase/guia_paso_a_paso_bpmn.md#4-errores-comunes-a-evitar).

## 📊 Rúbrica de Evaluación

| Criterio                            | Excelente (5)                                                       | Aceptable (3) / Insuficiente (1–2)                     |
|-------------------------------------|----------------------------------------------------------------------|---------------------------------------------------------|
| Claridad del diagrama BPMN          | Modelo limpio, con símbolos correctos y buena secuencia lógica       | Desordenado, símbolos incorrectos o secuencia confusa  |
| Representación del caso base        | Modelo representa adecuadamente el flujo propuesto (Clínica Salud Viva) | Modelo incompleto o incoherente con el caso de clase   |
| Aplicación al cliente real          | Se adapta adecuadamente el modelado al cliente con diferencias justificadas | No hay adaptación real o está desalineado              |
| Investigación complementaria        | Buenas prácticas BPMN aplicadas y bien citadas                       | Poco análisis o investigación desconectada              |

---

## ✅ Licencia

Este taller hace parte del curso de Arquitectura Empresarial - Universidad de La Sabana. Uso académico bajo licencia MIT.
