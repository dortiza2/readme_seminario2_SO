# readme_seminario2_SO
Ejercicio practico para curso de Sistemas Operativos en Seminario de Privado 2

# 🧪 Actividad Webmin - Detención de Proceso Manual (Estudiante18)

## 📌 Resumen Ejecutivo

Se realizó el análisis del listado de procesos activos en un servidor Ubuntu 22.04 mediante el panel Webmin, identificando uno que pudiera ser detenido sin comprometer el funcionamiento del sistema. Se seleccionó el proceso `cron` con **PID 144**, se verificó su información y se procedió a finalizarlo correctamente desde la interfaz.

---

## 🖥️ Entorno de Trabajo

| Elemento         | Detalle                      |
|------------------|------------------------------|
| Sistema Operativo| Ubuntu 22.04                 |
| Webmin           | v2.401                       |
| Tema             | Authentic Theme v24.01       |
| Usuario          | estudiante18                 |
| Servidor         | ct-procesos (192.168.4.105)  |

---

## 🧭 Procedimiento Paso a Paso

### 1. Ingreso al panel Webmin
Acceso al panel de administración vía navegador web utilizando credenciales de estudiante.

<img width="1174" alt="imagen" src="https://github.com/user-attachments/assets/86bd2110-3c8b-4e3c-997f-e98723956521" />
<img width="1860" alt="imagen" src="https://github.com/user-attachments/assets/f2a6d82c-a0dd-416e-ae85-54c8253cf853" />

---

### 2. Acceso a la sección de procesos
Navegación a **System > Running Processes** para visualizar los procesos activos del sistema.

📸 **[Ver captura](https://drive.google.com/file/d/1BpCc830y8UbT0XvROd4sQTH7G4JytS7U/view?usp=sharing)**

---

### 3. Análisis de procesos disponibles
Se revisó la lista para identificar procesos no críticos. Se evitó interactuar con servicios como `Webmin`, `systemd`, `nginx`, `postfix`, entre otros.

📸 **[Ver captura](https://drive.google.com/file/d/1Nfq2CYc-FYUgZylOSQQ9dtGKUCKJXcwx/view?usp=sharing)**
📸 **[Ver captura](https://drive.google.com/file/d/1Jap-AIi-3pkYqxYtHxp6sesRGqhPge7i/view?usp=sharing)**

---

### 4. Selección de proceso mediante ID
Se eligió el proceso con **PID 144**, correspondiente a `cron`. Se accedió a su detalle haciendo clic sobre su ID para obtener información adicional.

📸 **[Ver captura](https://drive.google.com/file/d/1FejendDEJ3C3HnB3ha33jTuUw_GpKUQm/view?usp=sharing)**

---

### 5. Finalización del proceso
Desde la pantalla de información del proceso se utilizó el botón **"Kill"** para detenerlo manualmente.

📸 **[Ver captura](https://drive.google.com/file/d/1GxYVLevkt3xPItgTHtAMVZM4Tlqb8dyR/view?usp=sharing)**

---

### 6. Verificación post-eliminación
Se actualizó la vista de procesos para comprobar que el proceso ya no se encontraba activo.

📸 **[Ver captura](https://drive.google.com/file/d/1hpAjH-WeOAZ9WjeVo2SCqQujGmzF1B_5/view?usp=sharing)**

---

## ✅ Resultado

- Proceso `cron` (PID 144) eliminado exitosamente.
- El sistema se mantuvo estable y funcional después de la operación.
- Se garantizó que ningún servicio crítico fuera afectado.

---

## ⚠️ Recomendaciones

- No detener procesos esenciales del sistema (`systemd`, `sshd`, `webmin`, `nginx`, etc.).
- Antes de finalizar un proceso, validar su función mediante nombre, ruta y usuario.
- Documentar todo el procedimiento y respaldar con capturas.
- Realizar estas acciones únicamente en entornos de pruebas o con autorización expresa.

---

## ✍️ Elaborado por
**Usuario:** David Alberto Ortiz Aquino 
**Fecha:** Junio 2025  
**Actividad:** Análisis y control de procesos en Webmin
