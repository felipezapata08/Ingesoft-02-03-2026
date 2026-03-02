## RF-02 - Agendar Cita

### HU-02 - Agendar Cita

**Descripción:**
Permite a un paciente registrado seleccionar y confirmar una cita médica en un horario disponible.

**Actor principal:** 
Paciente

**Precondición:**
El paciente debe estar autenticado y deben existir horarios disponibles en el sistema.

**Postcondición:**
La cita queda registrada en el sistema y el horario seleccionado queda reservado.

#### Historia de Usuario

Como paciente quiero seleccionar fecha y horario disponible para recibir atención médica.

#### Criterios de Aceptación
1. Solo los pacientes registrados y autenticados pueden agendar una cita.
2. El sistema debe mostrar unicamente los horarios disponibles al momento de agendar.
3. Una vez confirmada la cita, el sistema debe enviar una confirmación al paciente.
4. El horario seleccionado debe quedar bloqueado para otros pacientes tras la confirmación.
