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
