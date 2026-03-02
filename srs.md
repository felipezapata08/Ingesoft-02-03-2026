RNF
RNF-01 Disponibilidad:
El sistema debe estar disponible 24/7.
RNF-02 Seguridad:
Los datos médicos deben almacenarse de forma confidencial y cumplir con las normativas de protección de datos vigentes.
RNF-03 Rendimiento:
La cancelación de la cita debe procesarse en un tiempo máximo de 2 segundos.
RNF-04 Usabilidad:
La interfaz debe ser clara e intuitiva, permitiendo cancelar la cita en un máximo de 3 pasos.
Precondición:
El paciente debe estar autenticado y tener una cita previamente registrada.
Postcondición:
La cita queda cancelada en el sistema y el horario asociado vuelve a estar disponible para otros pacientes.
Historia de Usuario
Como paciente
quiero cancelar una cita previamente agendada
para liberar el espacio reservado
Criterios de Aceptación
Solo el paciente propietario de la cita puede cancelarla.
El sistema no debe permitir la cancelación después del tiempo límite definido por la clínica.
Al cancelar la cita, el horario debe quedar nuevamente disponible.
El sistema debe mostrar un mensaje de confirmación de cancelación exitosa.
El sistema debe registrar la fecha y hora en que se realizó la cancelación.
