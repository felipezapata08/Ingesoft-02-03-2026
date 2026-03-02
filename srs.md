## RF-03 – Cancelar Cita

### HU-03 – Cancelar Cita

**Descripción:**  
Permite a un paciente cancelar una cita médica previamente agendada.

**Actor principal:** Paciente

**Precondición:**  
El paciente debe estar autenticado y tener una cita previamente registrada.

**Postcondición:**  
La cita queda cancelada en el sistema.

#### Historia de Usuario

Como paciente  
quiero cancelar una cita previamente agendada  
para liberar el espacio reservado

#### Criterios de Aceptación

1. Solo el paciente propietario de la cita puede cancelarla.
2. El sistema no debe permitir la cancelación después del tiempo límite definido por la clínica.
3. Al cancelar la cita, el horario debe quedar nuevamente disponible.
4. El sistema debe mostrar un mensaje de confirmación de cancelación exitosa.
