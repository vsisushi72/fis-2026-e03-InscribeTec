**Proyecto:** InscribeTec
**Sección del proceso asignada:** Consulta de oferta académica y selección interactiva de materias en el horario (RF-03 y RF-04) 
**Rol principal de la U3:** Calidad y Documentación
**Fecha:** 2026-11-10

## 1. Información que necesito obtener

**Pregunta 1:** ¿De qué manera y con qué frecuencia Servicios Escolares o las Jefaturas de División actualizan la oferta de materias disponibles (grupos, días y horarios de clase) antes de abrir el periodo de inscripción para cada semestre?

**Pregunta 2:** ¿Qué ocurre en la operación actual cuando un alumno intenta seleccionar dos materias que se empalman en el mismo día y hora, o cuando el cupo de un grupo se llena mientras el alumno está armando su propuesta de horario?

**Técnica elegida y motivo:** Entrevista estructurada y revisión documental con el personal encargado, porque nos permite validar cómo se publican y filtran las materias por semestre hoy en día y confirmar qué validaciones de calidad o restricciones de horario deben aplicarse antes de dar por definitivos los requisitos.

**Fuente a consultar:** Encargado de Servicios Escolares y Jefatura de División de Ingeniería en Sistemas Computacionales del Instituto Tecnológico Superior de San Pedro de las Colonias.

**Fecha prevista o estado:** Pendiente de validar

## 2. Información que ya tengo

**Fuente real:** Documento del modelo de negocio U2-E01_InscribeTec_ModeloNegocio.pdf (07/10/2026, registrado como F-02) y la especificación del equipo U3-E01_InscribeTec_Requisitos.md (17/11/2026, junto con el diseño de pantallas en Figma). **Hallazgo comprobable:** Una vez que el alumno valida su acceso en la plataforma, pasa a la vista principal "Arma tu horario", donde el sistema le despliega la oferta de materias correspondientes a su semestre detallando los días y horas de clase asignados (RF-03). En el prototipo en Figma, el alumno puede interactuar directamente con la lista marcando o desmarcando las casillas de las materias de su interés, reflejándose de manera inmediata y dinámica únicamente las asignaturas seleccionadas dentro de su propuesta visual de horario (RF-04).

**Dudas:** Confirmar si el sistema mostrará al alumno todas las materias abiertas de la carrera o si filtrará automáticamente únicamente las materias que le corresponden cursar según su retícula y semestre vigente.

## 3. Necesidad identificada

De acuerdo con las necesidades (F-02 / N-02), las reglas del negocio y la lista de requisitos (Sección E) del documento más reciente del equipo, lo que se necesita resolver en mi parte del proceso es lo siguiente:

- **Presentar la oferta académica disponible (F-02 / N-02 / RF-03):** Garantizar que el alumno autenticado visualice de forma clara y ordenada la lista de materias disponibles para su semestre, incluyendo obligatoriamente sus días y horas de clase para darle la información base necesaria para armar su horario (prioridad alta P1).
    
- **Permitir la configuración interactiva de la carga académica (F-02 / N-02 / RF-04):** Asegurar que el alumno pueda marcar y desmarcar las materias de la lista disponible, integrando únicamente aquellas que haya seleccionado dentro de su propuesta de horario en tiempo real y sin duplicidades (prioridad alta P1).
    
- **Claridad visual y accesibilidad en la selección (RNF-01):** Verificar que el estado de selección (marcada/desmarcada) y la vista previa del horario sean comprensibles mediante texto e indicadores visuales claros, sin depender exclusivamente de cambios de color.
    

## 4. Referencias y fuentes utilizadas

Fuentes del proyecto

- U3-E01_InscribeTec_Requisitos.md (Apartado A: Alcance, Apartado B: Fuentes y necesidad [F-02, N-02], Apartado D: Reglas del dominio, Apartado E: Lista de requisitos [RF-03, RF-04, RNF-01], Apartado F: Pruebas y Apartado G: Pantallas del diseño).
    
- U2-E01_InscribeTec_ModeloNegocio.pdf (Apartado A: Acuerdo del equipo — Datos de entrada, procesamiento y salida del proceso de inscripción).
    
- Prototipo en Figma: InscribeTec – Recorrido prioritario ([https://www.figma.com/design/5rvYS8nPekkjX8vKgHIj1Q/Untitled?node-id=0-1&p=f&t=ttbn5w9Gd4FOMrUb-0](https://www.figma.com/design/5rvYS8nPekkjX8vKgHIj1Q/Untitled?node-id=0-1&p=f&t=ttbn5w9Gd4FOMrUb-0), Pantalla "Arma tu horario" — Listado de materias disponibles y propuesta de horario).
    

### Declaración de uso de IA

- **Herramienta utilizada:** Gemini, utilizado para apoyar la estructura y corrección ortográfica del documento.