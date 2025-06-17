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

<img width="442" alt="Imagen 2" src="https://github.com/user-attachments/assets/eef08a2b-13e4-45e9-af53-290efa0cae54" />
<img width="253" alt="Imagen 2_2" src="https://github.com/user-attachments/assets/6f0ee83a-0554-447d-af7a-e989d40854da" />


---

### 3. Análisis de procesos disponibles
Se revisó la lista para identificar procesos no críticos. Se evitó interactuar con servicios como `Webmin`, `systemd`, `nginx`, `postfix`, entre otros.

<img width="442" alt="Imagen 3" src="https://github.com/user-attachments/assets/7c473a8a-a628-4442-8fec-dccc3c3180b6" />
<img width="1582" alt="Imagen 3_3" src="https://github.com/user-attachments/assets/3e5fe655-e0b4-4c4b-9ad1-1cee23432807" />

---

### 4. Selección de proceso mediante ID
Se eligió el proceso con **PID 144**, correspondiente a `cron`. Se accedió a su detalle haciendo clic sobre su ID para obtener información adicional.

<img width="442" alt="Imagen 4" src="https://github.com/user-attachments/assets/cc1ea1ba-dc88-44af-9708-bd9b3b1f0fc8" />


---

### 5. Finalización del proceso
Desde la pantalla de información del proceso se utilizó el botón **"Kill"** para detenerlo manualmente.

<img width="442" alt="Imagen 5" src="https://github.com/user-attachments/assets/13938905-dfdf-44d8-b119-8a6251281ba3" />
<img width="700" alt="Imagen 5_5" src="https://github.com/user-attachments/assets/5b0c49b8-0bde-42e0-9ab4-401cff215a7a" />

---

### 6. Verificación post-eliminación
Se actualizó la vista de procesos para comprobar que el proceso ya no se encontraba activo.

<img width="442" alt="Imagen 6" src="https://github.com/user-attachments/assets/676b4e4d-756d-48b3-887a-91d2855b75c8" />
<img width="1017" alt="Imagen 6_6" src="https://github.com/user-attachments/assets/cb067f13-6d37-4f01-94e7-73494c0bbed2" />

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
