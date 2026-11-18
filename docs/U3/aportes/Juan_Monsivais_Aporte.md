# Aporte individual – Juan Monsivais

**Proyecto:** InscribeTec
**Sección del proceso asignada:** Validación de pago previo acreditado y confirmación formal del horario semestral (`RF-05`, `RF-06`)
**Rol principal de la U3:** Coordinación
**Fecha:** 2026-11-15

## 1. Información que necesito obtener
- Pregunta 1: ¿Cómo se refleja en el sistema escolar el estatus de pago validado para habilitar la confirmación del horario?
- Pregunta 2: ¿Qué mensaje o restricción exacta aplica Servicios Escolares cuando un alumno intenta inscribir materias sin tener su pago acreditado?
- Técnica elegida y motivo: Entrevista semiestructurada y análisis documental de evidencias previas del equipo (`C6-A01` y `U2-E01`), ya que permiten confirmar las reglas administrativas reales sin suponer flujos de cobro.
- Fuente a consultar: Personal Administrativo / Servicios Escolares del Tecnológico de San Pedro de las Colonias y documentos base de U1/U2.
- Fecha prevista o estado: Confirmado mediante respaldo documental de documentos base de U1/U2.

## 2. Información que ya tengo
- Fuente real: `F-01` (`PasoLibre_C6-A01_Investigacion.pdf`, 2026-09-15) y `F-02` (`U2-E01_InscribeTec_ModeloNegocio.pdf`, 2026-10-07).
- Hallazgo comprobable: El alumno realiza el pago por medios externos (tarjeta en el Instituto, cajero inteligente BBVA o app BBVA). La plataforma `InscribeTec` no procesa pagos ni sube comprobantes, sino que verifica que el pago esté acreditado antes de permitir confirmar el horario armado (`RG-01`).
- Dudas: Falta validar con Servicios Escolares el tiempo de actualización del estatus de pago entre el banco y el sistema escolar.

## 3. Necesidad identificada
- **`N-02`:** Permitir al alumno seleccionar sus materias disponibles, confirmar su carga y consultar su horario semanal en línea (`F-01`, `F-02`).
- **`N-03`:** Asegurar que el horario solo pueda confirmarse cuando el alumno cuente con su pago previo acreditado en el sistema (`F-01`).

## 4. Requisitos propuestos y criterios de aceptación

### `RF-05` — Confirmación de horario con pago previo acreditado
- **Tipo:** Funcional (RF)
- **Enunciado verificable:** El sistema debe permitir al alumno confirmar su horario armado con las materias marcadas cuando su estatus de pago previo se encuentre acreditado.
- **Fuente:** `F-01`, `F-02` / `N-02`
- **Prioridad:** P1 — Es indispensable para formalizar la selección de materias del estudiante y completar el recorrido principal.
- **Estado:** Propuesto / Confirmado
- **Criterio de aceptación:**
  - **Condición (Dado):** El alumno se encuentra autenticado en `02. Acción · Arma tu horario`, tiene al menos una materia marcada y su estatus de pago previo aparece como acreditado.
  - **Acción (Cuando):** Presiona el botón **"Confirmar horario"**.
  - **Resultado esperado (Entonces):** El sistema registra la carga académica, muestra la vista `03A. Éxito · Confirmación de horario` y habilita la visualización en `04. Resultado · Mi horario`.

### `RF-06` — Bloqueo de confirmación y aviso por pago no realizado
- **Tipo:** Funcional (RF)
- **Enunciado verificable:** El sistema debe impedir la confirmación del horario y mostrar en texto un aviso indicando que el pago no ha sido realizado cuando el alumno tenga pendiente dicho requisito previo.
- **Fuente:** `F-01` / `N-03` (`RG-01`)
- **Prioridad:** P1 — Garantiza el cumplimiento de la regla institucional de elegibilidad previa (`RG-01`).
- **Estado:** Propuesto / Confirmado
- **Criterio de aceptación:**
  - **Condición (Dado):** El alumno se encuentra autenticado en `02. Acción · Arma tu horario`, tiene materias marcadas pero su estatus de pago previo figura como no realizado.
  - **Acción (Cuando):** Presiona el botón **"Confirmar horario"** (o activa la simulación de pago pendiente).
  - **Resultado esperado (Entonces):** El sistema bloquea la confirmación, impide avanzar a `04. Resultado · Mi horario` y despliega un aviso claro en texto en `03B. Error` indicando que el pago no ha sido realizado (`RNF-01`).
