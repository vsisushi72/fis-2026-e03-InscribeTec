# Aporte individual — Luis Fernando Villalobos Hernández

- **Proyecto:** InscribeTec
- **Sección del proceso asignada:** Consulta del horario armado de lunes a viernes y control de acceso por sesión del alumno (RF-07, RNF-01)
- **Rol principal de la U3:** Calidad y Documentación
- **Fecha:** 2026-11-17

## 1. Información que necesito obtener

- **Pregunta 1:** ¿Qué datos exactos debe visualizar el alumno en su horario final (nombre de la materia, docente, aula, grupo, horario) y qué formato de comprobante oficial recibe tras confirmar su carga académica?
- **Pregunta 2:** ¿De qué manera o mediante qué registro el área de Finanzas confirmará en el sistema qué alumnos ya cuentan con el pago realizado para habilitar la confirmación de su horario?
- **Técnica elegida y motivo:** Consulta directa / entrevista semiestructurada con el personal operativo, porque permite confirmar los datos exactos que exige la institución en el comprobante de horario y el mecanismo real de validación de pagos antes de cerrar la especificación.
- **Fuente a consultar:** Encargado de Servicios Escolares y encargado de Finanzas del Tecnológico de San Pedro de las Colonias.
- **Fecha prevista o estado:** Pendiente de validar

## 2. Información que ya tengo

- **Fuente real:** Investigación previa C6-A01 (`PasoLibre_C6-A01_Investigacion.pdf`, 2026-09-15) y Modelo de Negocio (`U2-E01_InscribeTec_ModeloNegocio.pdf`, 2026-10-07).
- **Hallazgo comprobable:** En U2-E01 (F-02) se estableció que las entradas del proceso son las credenciales del alumno y la salida principal es su horario y comprobante de inscripción. En el recorrido del prototipo diseñado en Figma (Pantalla 3A · Mi horario), el alumno consulta una tabla de lunes a viernes únicamente con las materias que seleccionó previamente, y el acceso está restringido mediante la validación de su número de control y CURP.
- **Dudas:** Confirmar si el horario desplegado en pantalla requiere incluir información adicional (como nombre del profesor o salón), si el alumno debe poder descargarlo o imprimirlo en PDF, y cómo se sincronizará el estado de pago con Finanzas.

## 3. Necesidad identificada

- **N-01 (Privacidad y control de acceso por alumno — vinculada a RNF-01):** Garantizar que el sistema muestre a cada alumno únicamente su propia información de inscripción (como su CURP y carga académica) y solo después de haber iniciado sesión con credenciales válidas, impidiendo el acceso directo sin sesión o con la cuenta de otro estudiante.
- **N-02 (Visualización clara del horario armado — vinculada a RF-07):** Permitir que el alumno consulte de forma ordenada en una vista semanal (de lunes a viernes) únicamente las materias que marcó y confirmó, mostrando el horario correspondiente a cada una como salida principal del trámite.

## 4. Referencias y fuentes utilizadas

- `PasoLibre_C6-A01_Investigacion.pdf` (2026-09-15). Investigación del equipo Paso Libre sobre métodos de pago y flujo institucional de inscripción.
- `U2-E01_InscribeTec_ModeloNegocio.pdf` (2026-10-07). Definición de entradas, salidas y recorrido TO-BE del proyecto InscribeTec.
- `U3-E01_InscribeTec_Requisitos.md` (v0.2, 2026-11-17). Plan de obtención (B1), fuentes consultadas (F-01, F-02), catálogo de requisitos (RF-07, RNF-01) y prototipo en Figma (Pantalla 3A · Mi horario).

## Declaración de uso de IA

- **Herramienta utilizada:** Gemini (asistente de IA), utilizado para apoyar en la síntesis de la información del proyecto y la estructuración del documento.