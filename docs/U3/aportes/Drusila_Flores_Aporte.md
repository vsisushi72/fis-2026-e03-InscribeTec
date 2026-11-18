# Aporte individual — Drusila Betsabé Flores Chávez
**Proyecto:** InscribeTec
**Sección del proceso asignada:** Inicio de sesión y validación de credenciales del alumno (RF-01 y RF-02)
**Rol principal de la U3:** Análisis
**Fecha:** 2026-10-28

## 1. Información que necesito obtener

**Pregunta 1:** ¿De dónde obtiene Servicios Escolares la lista o registro de alumnos con su número de control y CURP para comprobar que sí pueden entrar a inscribirse?

**Pregunta 2:** ¿Qué pasa en la vida real si un alumno escribe bien sus datos, pero tiene algún error en su CURP o algún adeudo/bloqueo que no lo deje reinscribirse en ese semestre?

**Técnica elegida y motivo:** Plática o entrevista directa con el encargado, porque así podemos confirmar cómo revisan los datos de los alumnos hoy en día y qué casos especiales ocurren antes de dar por buenos nuestros requisitos.

**Fuente a consultar:** Encargado de Servicios Escolares del Tecnológico de San Pedro de las Colonias.

**Fecha prevista o estado:** Pendiente de validar

## 2. Información que ya tengo

**Fuente real:** Documento del modelo de negocio U2-E01_InscribeTec_ModeloNegocio.pdf (07/10/2026, registrado como F-02) y la especificación del equipo U3-E01_InscribeTec_Requisitos.md (17/11/2026, junto con el diseño de pantallas en Figma). **Hallazgo comprobable:** Para empezar su inscripción en la página, el alumno necesita entrar usando su número de control y su CURP. En el diseño en Figma, el alumno escribe ambos datos y presiona "Ingresar" (Pantalla 1): si los datos están bien, el sistema lo deja pasar a elegir sus materias en "Arma tu horario" (RF-01); si alguno está mal, no lo deja entrar y le muestra un aviso escrito explicando que sus datos no son válidos, sin depender solo del color rojo (Pantalla 2B, RF-02 y RNF-01).

**Dudas:** Confirmar si la página revisará los datos del alumno conectándose directo a la lista oficial de la escuela al momento, o si Servicios Escolares subirá una lista de alumnos antes de que empiecen las inscripciones.

## 3. Necesidad identificada

De acuerdo con las necesidades (F-02 / N-01), las reglas (RG-02) y la lista de requisitos (Sección E) del documento más reciente del equipo, lo que se necesita resolver en mi parte del proceso es lo siguiente: Comprobar quién entra a la página (F-02 / N-01): Asegurarnos de que la persona que entra a hacer el trámite realmente sea el alumno, pidiéndole su número de control y su CURP antes de dejarlo ver las materias. Dejar pasar al alumno si sus datos son correctos (RF-01 / RG-02): La página debe revisar que el número de control y la CURP coincidan con los de un alumno registrado para abrirle la pantalla "Arma tu horario" (prioridad alta P1), cumpliendo la regla de que solo los alumnos registrados pueden entrar. Detener el acceso y avisar con texto si hay un error (RF-02 / RNF-01): Si el número de control o la CURP están mal o no coinciden, la página debe dejar al alumno en la misma pantalla de inicio y mostrarle un mensaje claro escrito con palabras avisándole que sus datos son incorrectos (prioridad alta P1).

## 4. Referencias y fuentes utilizadas

Fuentes del proyecto

·        U3-E01_InscribeTec_Requisitos.md (Apartado A: Alcance, Apartado B: Fuentes y necesidades [F-02, N-01], Apartado D: Reglas [RG-02], Apartado E: Lista de requisitos [RF-01, RF-02, RNF-01], Apartado F: Pruebas y Apartado G: Pantallas del diseño).

·        U2-E01_InscribeTec_ModeloNegocio.pdf (Apartado A: Acuerdo del equipo — Datos de entrada y salida del proceso de inscripción). Prototipo en Figma: InscribeTec – Recorrido prioritario ([https://www.figma.com/design/5rvYS8nPekkjX8vKgHIj1Q/Untitled?node-id=0-1&p=f&t=ttbn5w9Gd4FOMrUb-0](https://www.figma.com/design/5rvYS8nPekkjX8vKgHIj1Q/Untitled?node-id=0-1&p=f&t=ttbn5w9Gd4FOMrUb-0), Pantalla 1 · Inicio de sesión y Pantalla 2B · Credenciales inválidas).

### Declaración de uso de IA

- **Herramienta utilizada:** Gemini (asistente de IA), utilizado para apoyar en la corrección ortográfica y sintaxis del documento.