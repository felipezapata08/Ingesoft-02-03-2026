# 🏥 Documentación de Requerimiento: Gestión de Citas

## 📌 RF-03 – Cancelar Cita
**HU-03 – Cancelar Cita**

---

### 📝 Descripción
Permite a un paciente cancelar una cita médica previamente agendada en el sistema de manera eficiente y segura.

### 👤 Actor Principal
* **Paciente**

---

### ⚙️ Requisitos No Funcionales (RNF)

| Código | Atributo | Descripción |
| :--- | :--- | :--- |
| **RNF-01** | **Disponibilidad** | El sistema debe estar disponible **24/7**. |
| **RNF-02** | **Seguridad** | Datos cifrados y cumplimiento de normativas de protección de datos. |
| **RNF-03** | **Rendimiento** | Tiempo de procesamiento máximo de **2 segundos**. |
| **RNF-04** | **Usabilidad** | Interfaz clara; cancelación en un máximo de **3 pasos**. |

---

### 🔐 Reglas de Control (Pre y Post)

> **Precondición:** > El paciente debe estar **autenticado** en la plataforma y poseer al menos una **cita activa** registrada.

> **Postcondición:** > La cita cambia a estado `CANCELADA`. El horario se libera automáticamente en la agenda médica para otros pacientes.

---

### 📖 Historia de Usuario

**COMO** paciente  
**QUIERO** cancelar una cita previamente agendada  
**PARA** liberar el espacio reservado y evitar penalizaciones.

#### ✔️ Criterios de Aceptación
1.  **Validación de Identidad:** Solo el paciente propietario de la cita puede realizar la acción.
2.  **Restricción de Tiempo:** No se permite cancelar si se supera el tiempo límite definido (ej. menos de 24h antes).
3.  **Actualización de Inventario:** El horario debe quedar disponible inmediatamente tras la acción.
4.  **Feedback al Usuario:** Mostrar un mensaje claro de "Cancelación Exitosa".
5.  **Auditoría:** El sistema debe registrar un log con la **fecha y hora exacta** de la transacción.

---

### 🛠️ Flujo Sugerido del Sistema (UX)
1. **Paso 1:** Acceder al módulo "Mis Citas".
2. **Paso 2:** Seleccionar cita y hacer clic en "Cancelar".
3. **Paso 3:** Confirmar en la ventana emergente.
