# U3 · Especificación de Requisitos - InscribeTec

**Versión:** 0.2  
**Fecha:** 17 de noviembre de 2026  
**Equipo y roles:**
- Juan Antonio Monsivais Fuantos (Coordinación)
- Drusila Betsabé Flores Chávez (Análisis)
- Luis Fernando Villalobos Hernández (Desarrollo)
- Britany Gisell Olivares Méndez (Calidad y Documentación) - Responsable de Revisión

**Estado del documento:** En elaboración

## A. Identificación y alcance

- **Proyecto:** InscribeTec, Tecnológico de San Pedro de las Colonias.
- **Proceso TO-BE seleccionado:** Armado, confirmación y consulta del horario de la inscripción semestral en línea (recorrido principal del prototipo en Figma).
- **Objetivo de esta especificación:** Definir los requisitos que sustentan el recorrido principal del prototipo: iniciar sesión, armar el horario, confirmarlo y consultarlo, incluidos los casos de credenciales inválidas y de pago no realizado.
- **Dentro del alcance:**
  - Inicio de sesión del alumno con número de control y CURP, con aviso de credenciales inválidas.
  - Selección de materias para armar el horario.
  - Confirmación del horario, con aviso cuando no se ha cumplido con el pago.
  - Consulta del horario armado, de lunes a viernes.
- **Fuera del alcance:**
  - Realización del pago (el alumno lo hace con tarjeta en el Tec, en cajero inteligente BBVA o en la app BBVA).

### Aportaciones por integrante

| Nombre                             | Rol U3                  | Dos IDs asignados | Enlace Trello/PR              |
| ---------------------------------- | ----------------------- | ----------------- | ----------------------------- |
| Juan Antonio Monsivais Fuantos     | Coordinación            | RF-05, RF-06      | https://trello.com/c/leka5GPf |
| Drusila Betsabé Flores Chávez      | Análisis                | RF-01, RF-02      | https://trello.com/c/b014ILfm |
| Luis Fernando Villalobos Hernández | Desarrollo              | RF-07, RNF-01     | https://trello.com/c/Vg6tYyF7 |
| Britany Gisell Olivares Méndez     | Calidad y Documentación | RF-03, RF-04      | https://trello.com/c/hqs3kT3L |

## B. Fuentes y necesidades

### B1. Plan de obtención

| Pregunta por resolver                                                                                    | Persona o documento a consultar                    | Técnica                       | Responsable      | Estado    |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------- | ----------------------------- | ---------------- | --------- |
| ¿Qué datos validan la identidad del alumno (número de control y CURP) y contra qué registro se comparan? | Encargado de servicios escolares                   | Entrevista o consulta directa | Drusila Flores   | Pendiente |
| ¿Quién entrega los horarios y las materias disponibles al inicio del ciclo y en qué momento?             | Encargado de servicios escolares                   | Entrevista o consulta directa | Britany Olivares | Pendiente |
| ¿Puede el alumno elegir libremente sus materias o hay materias asignadas, seriación o límites?           | Jefe de carrera                                    | Entrevista o consulta directa | Britany Olivares | Pendiente |
| ¿Quién confirma el pago del alumno y con qué evidencia o sistema lo verifica?                            | Encargado de Finanzas                              | Entrevista o consulta directa | Juan Monsivais   | Pendiente |
| ¿Cómo se identifica a un alumno que no ha cumplido con el pago y qué debe hacer para regularizarse?      | Encargado de Finanzas                              | Entrevista o consulta directa | Juan Monsivais   | Pendiente |
| ¿Qué pasos presenciales son obligatorios para dar por terminada la inscripción?                          | Jefe de carrera y encargado de servicios escolares | Entrevista o consulta directa | Drusila Flores   | Pendiente |
| ¿Qué información debe ver el alumno en su horario final y qué comprobante recibe?                        | Encargado de servicios escolares                   | Entrevista o consulta directa | Luis Villalobos  | Pendiente |

### B2. Fuentes realmente consultadas

| ID   | Técnica o documento                             | Fecha       | Hallazgo o necesidad                                                                                                                                                                                                    | Estado                                           | Enlace o referencia                  |
| ---- | ----------------------------------------------- | ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ | ------------------------------------ |
| F-01 | Investigación C6-A01 (documento)                | 2026-09-15  | El alumno paga con tarjeta en el Tec, cajero inteligente BBVA o app BBVA, usando los datos de su ficha (monto, concepto y referencia); Finanzas revisa el pago.                                                         | Por validar                                      | PasoLibre_C6-A01_Investigacion.pdf   |
| F-02 | Modelo de negocio U2-E01 (documento del equipo) | 2026-10-07  | La entrada del proceso son las credenciales del alumno; la salida es su horario y su comprobante de inscripción; inicia con la ficha de pago y termina cuando el alumno queda inscrito y se le entregan sus documentos. | Antecedente del equipo; por validar con usuarios | U2-E01_InscribeTec_ModeloNegocio.pdf |


### B3. Necesidades identificadas

| ID   | Necesidad                                                                                                 | Fuente | Estado      |
| ---- | --------------------------------------------------------------------------------------------------------- | ------ | ----------- |
| N-01 | Confirmar que quien entra al sistema es el alumno, mediante sus credenciales (número de control y CURP). | F-02   | Por validar |
| N-02 | Que el alumno obtenga su horario de inscripción.                                                          | F-02   | Por validar |
| N-03 | Que el horario solo pueda confirmarse cuando el pago esté cumplido.                                       | F-01   | Por validar |

### B4. Pendientes

| Pendiente                                                                                              | Fuente por consultar                  | Responsable      |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------- | ---------------- |
| Confirmar quién verifica el pago y con qué evidencia.                                                  | Encargado de finanzas                 | Juan Monsivais   |
| Confirmar los pasos presenciales obligatorios (por ejemplo, la firma de las hojas de carga académica). | Jefe de carrera y servicios escolares | Drusila Flores   |
| Obtener las materias y horarios reales del semestre (los del prototipo son de ejemplo).                | Servicios escolares                   | Britany Olivares |
| Definir el como se puede imprimir la carga academica una vez confirmado el horario.                    | Servicios escolares                   | Juan Monsivais   |
| Obtener la informacion sobre como se va a confirmar cuales alumnos cuentan con el pago ya realizado    | Encargado de finanzas                 | Luis Villalobos  |

## C. Organización del alcance

- **Ruta elegida:** Ruta B (requisitos directos)
- **Motivo de elección:** El recorrido es un proceso acotado de un solo tipo de usuario (el alumno) y pocas funciones: iniciar sesión, armar el horario, confirmarlo y consultarlo. No hace falta agruparlo en una épica.
- **Proceso:** Armar y consultar el horario de inscripción semestral.
- **Objetivo:** Permitir al alumno entrar con sus credenciales, elegir sus materias, confirmar su horario y consultarlo.
- **Requisitos vinculados:** RF-01, RF-02, RF-03, RF-04, RF-05, RF-06, RF-07, RNF-01.

## D. Reglas del dominio

| ID    | Regla del contexto                                                                                               | Quién la establece                    | Origen en B2              | Estado      |
| ----- | ---------------------------------------------------------------------------------------------------------------- | ------------------------------------- | ------------------------- | ----------- |
| RG-01 | El alumno que no ha cumplido con el pago no puede confirmar su horario.                                          | Jefe de carrera y servicios escolares | Origen pendiente · ver B4 | Por validar |
| RG-02 | Solo el alumno con credenciales válidas (número de control y CURP que coincidan) puede acceder a su inscripción. | Servicios escolares                   | Origen pendiente · ver B4 | Por validar |

## E. Catálogo de requisitos priorizado

| ID     | Tipo         | Requisito verificable                                                                                                                                                                   | Origen (F / N) | Prioridad | Motivo                                                                                         | Autor            | Estado    |
| ------ | ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | --------- | ---------------------------------------------------------------------------------------------- | ---------------- | --------- |
| RF-01  | Funcional    | El sistema debe permitir al alumno acceder al armado de su horario cuando el número de control y la CURP ingresados coincidan con un registro de alumno.                                | F-02 / N-01    | P1        | Sin acceso validado no se puede iniciar el trámite.                                            | Drusila Flores   | Propuesto |
| RF-02  | Funcional    | El sistema debe mantener al alumno en la pantalla de inicio de sesión y mostrar en texto que las credenciales son inválidas cuando el número de control y la CURP no coincidan.         | F-02 / N-01    | P1        | Evita que avance quien no demuestra ser el alumno.                                             | Drusila Flores   | Propuesto |
| RF-03  | Funcional    | El sistema debe mostrar al alumno la lista de materias disponibles para armar su horario, con su horario de clase.                                                                      | F-02 / N-02    | P1        | Sin la lista de materias el alumno no puede armar su horario.                                  | Britany Olivares | Propuesto |
| RF-04  | Funcional    | El sistema debe permitir al alumno marcar y desmarcar las materias de la lista, de modo que solo las materias marcadas formen parte de su horario.                                       | F-02 / N-02    | P1        | Sin selección no hay horario que confirmar ni consultar.                                       | Britany Olivares | Propuesto |
| RF-05  | Funcional    | El sistema debe permitir al alumno confirmar el horario armado con las materias que marcó.                                                                                              | F-02 / N-02    | P1        | Es el paso que formaliza la elección del alumno.                                               | Juan Monsivais   | Propuesto |
| RF-06  | Funcional    | El sistema debe impedir la confirmación del horario y mostrar en texto un aviso de que no se ha cumplido con el pago cuando el alumno tenga un pago pendiente.                           | F-01 / N-03    | P1        | Es una regla esencial: sin pago no se confirma el horario (RG-01).                             | Juan Monsivais   | Propuesto |
| RF-07  | Funcional    | El sistema debe mostrar al alumno su horario armado, de lunes a viernes, solo con las materias que marcó y la hora de cada una.                                                          | F-02 / N-02    | P1        | Es la salida principal del proceso.                                                            | Luis Villalobos  | Propuesto |
| RNF-01 | No Funcional | El sistema debe mostrar a cada alumno únicamente su propia información de inscripción y solo después de que inicie sesión con credenciales válidas.                                       | F-02 / N-01    | P1        | Protege los datos personales del alumno (como su CURP) y evita que otra persona vea su horario. | Luis Villalobos  | Propuesto |

## F. Criterios de aceptación

| Requisito ID | Entrada o Condición                                                            | Acción                                                             | Resultado Esperado Observable                                                                                |
| ------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| RF-01        | Número de control y CURP que coinciden con un registro de alumno.              | Presionar el botón "Ingresar".                                     | El sistema muestra la pantalla "Arma tu horario".                                                            |
| RF-02        | Número de control y CURP que no coinciden con ningún registro.                 | Presionar el botón "Ingresar".                                     | El alumno permanece en el inicio de sesión y aparece un texto que indica que las credenciales son inválidas. |
| RF-03        | Alumno con sesión iniciada.                                                    | Entrar a la pantalla "Arma tu horario".                            | Se muestran las cinco materias disponibles, cada una con su horario.                                         |
| RF-04        | Lista de materias mostrada.                                                    | Marcar o desmarcar una materia.                                    | La casilla de la materia cambia de estado y solo las materias marcadas pasan al horario.                     |
| RF-05        | Alumno con al menos una materia marcada y sin pago pendiente.                  | Presionar "Confirmar horario".                                     | Se verifica que se cuente con los requisitos, si cumple se le otorga su carga academica                      |
| RF-06        | Alumno con pago pendiente y materias marcadas.                                 | Presionar "Confirmar horario".                                     | El horario no se confirma y aparece un texto que indica que no se ha cumplido con el pago.                   |
| RF-07        | Alumno con materias marcadas.                                                  | Presionar "Ver horario".                                           | Se muestra una tabla de lunes a viernes solo con las materias marcadas.                                      |
| RNF-01       | Usuario sin sesión iniciada, o alumno con la sesión de otro número de control. | Intentar abrir directamente la pantalla "Mi horario" de un alumno. | El sistema no muestra el horario y envía al usuario al inicio de sesión.                                     |

## G. Backlog y boceto

### Tabla del Backlog (Orden por Prioridad)

| Orden | ID Requisito | Prioridad | Dependencia | Tarjeta Trello                | Boceto Asociado                        |
| ----- | ------------ | --------- | ----------- | ----------------------------- | -------------------------------------- |
| 1     | RF-01        | P1        | Ninguna     | https://trello.com/c/deH9YDHt | Pantalla 1 · Inicio de sesión          |
| 2     | RF-02        | P1        | RF-01       | https://trello.com/c/T7GoWRr1 | Pantalla 2B · Credenciales inválidas   |
| 3     | RNF-01       | P1        | RF-01       |                               | No representable en boceto (seguridad) |
| 4     | RF-03        | P1        | RF-01       | https://trello.com/c/RnoDFKuk | Pantalla 2A · Armar horario            |
| 5     | RF-04        | P1        | RF-03       | https://trello.com/c/RnoDFKuk | Pantalla 2A · Armar horario            |
| 6     | RF-05        | P1        | RF-04       | https://trello.com/c/RnoDFKuk | Pantalla 2A · Armar horario            |
| 7     | RF-06        | P1        | RF-05       | https://trello.com/c/lOQ19E0v | Pantalla 2C · Pago pendiente           |
| 8     | RF-07        | P1        | RF-04       | https://trello.com/c/CZVaEUvX | Pantalla 3A · Mi horario               |

### Boceto del Recorrido Prioritario

- **Prototipo en Figma:** https://www.figma.com/design/5rvYS8nPekkjX8vKgHIj1Q/Untitled
- **Ubicación del archivo en el repositorio:** `docs/U3/prototipo/` ([completar: nombre del archivo]).
- **Estado:** Borrador · pendiente de validar. Las materias y horarios del prototipo son de ejemplo.

| Bloque         | Pantalla del prototipo               | Qué muestra                                                                                                           | Requisitos          |
| -------------- | ------------------------------------ | --------------------------------------------------------------------------------------------------------------------- | ------------------- |
| 01 · Inicio    | Pantalla 1 · Inicio de sesión        | Campos de número de control y CURP, y botón "Ingresar".                                                               | RF-01               |
| 02 · Acción    | Pantalla 2A · Armar horario          | Lista de cinco materias con casilla, y los botones "Confirmar horario" y "Ver horario".                               | RF-03, RF-04, RF-05 |
| 03A · Éxito    | Pantalla 2D · Horario confirmado     | Mensaje de confirmación exitosa de la carga académica con las materias seleccionadas y botón para ir a "Ver horario". | RF-05               |
| 03B · Error    | Pantalla 2B · Credenciales inválidas | Aviso en texto de credenciales inválidas.                                                                             | RF-02               |
| 03B · Error    | Pantalla 2C · Pago pendiente         | Aviso en texto de que no se ha cumplido con el pago.                                                                  | RF-06               |
| 04 · Resultado | Pantalla 3A · Mi horario             | Tabla de lunes a viernes con las materias marcadas.                                                                   | RF-07               |

## H. Trazabilidad y cambios

### Matriz de Trazabilidad

| Fuente (B2) | Necesidad (B3) | ID (E) | Criterio (F) | Boceto o comprobación (G)                                                                   |
| ----------- | -------------- | ------ | ------------ | ------------------------------------------------------------------------------------------- |
| F-02        | N-01           | RF-01  | F · RF-01    | Pantalla 1 · Inicio de sesión                                                               |
| F-02        | N-01           | RF-02  | F · RF-02    | Pantalla 2B · Credenciales inválidas                                                        |
| F-02        | N-02           | RF-03  | F · RF-03    | Pantalla 2A · Armar horario                                                                 |
| F-02        | N-02           | RF-04  | F · RF-04    | Pantalla 2A · Armar horario                                                                 |
| F-02        | N-02           | RF-05  | F · RF-05    | Pantalla 2A · Armar horario                                                                 |
| F-01        | N-03           | RF-06  | F · RF-06    | Pantalla 2C · Pago pendiente                                                                |
| F-02        | N-02           | RF-07  | F · RF-07    | Pantalla 3A · Mi horario                                                                    |
| F-02        | N-01           | RNF-01 | F · RNF-01   | No representable en boceto; prueba propuesta: intentar abrir el horario sin sesión iniciada |

### Registro de cambios

| Fecha      | Motivo                                                                              | IDs afectados | Decisión                                                                                  |
| ---------- | ----------------------------------------------------------------------------------- | ------------- | ----------------------------------------------------------------------------------------- |
| 2026-11-10 | Integración de aportes individuales de obtención de requisitos en ramas personales. | Todos         | Se documentan las necesidades y hallazgos base (v0.1) previo al prototipado.              |
| 2026-11-17 | Se rehace el E01 a partir del prototipo realizado en Figma.                         | Todos         | La versión 0.2 sustituye a la versión 0.1 para alinear requisitos, criterios y pantallas. |

## I. Referencias y herramientas

### Fuentes de información

| Fuente                                | Autor u organización | Fecha       | Referencia                           | Fecha de consulta |
| ------------------------------------- | -------------------- | ----------- | ------------------------------------ | ----------------- |
| Investigación C6-A01                  | Equipo Paso Libre    | 2026-09-15  | PasoLibre_C6-A01_Investigacion.pdf   | [completar]       |
| Modelo de negocio U2-E01              | Equipo Paso Libre    | 2026-10-07  | U2-E01_InscribeTec_ModeloNegocio.pdf | [completar]       |


### Herramientas y recursos

| Herramienta | Proveedor    | Uso real                                                                                                | Enlace oficial                            | Fecha de consulta |
| ----------- | ------------ | ------------------------------------------------------------------------------------------------------- | ----------------------------------------- | ----------------- |
| Figma       | Figma, Inc.  | Prototipo interactivo de baja fidelidad del recorrido.                                                  | https://www.figma.com                     | 12-11-2026        |
| Claude (IA) | Anthropic    | Apoyo para correcciones en ortograficas y estructurado del documento                                    | https://claude.ai                         | 15-11-2026        |
| Trello      | Atlassian    | Gestión del backlog, asignación de tareas (`[ACT-56]` a `[ACT-81]`) y seguimiento Kanban.               | https://trello.com/u/drusilaflores/boards | 17-11-2026        |
| GitHub      | GitHub, Inc. | Control de versiones, ramas individuales, revisión cruzada mediante PRs y alojamiento de documentación. | https://github.com/                       | 17-11-2026        |

**Qué se verificó del uso de IA:** La inteligencia artificial se utilizó únicamente como apoyo puntual para revisar ortografía y dar formato a la sintaxis del texto ya redactado por el equipo; se verificó manualmente que las sugerencias menores no alteraran el sentido técnico de nuestros requisitos (`RF-01` a `RNF-01`), que no incluyeran información ajena a nuestras fuentes reales (`F-01` y `F-02`) ni entrevistas pendientes, y que coincidieran exactamente con el prototipo diseñado por el equipo en Figma.