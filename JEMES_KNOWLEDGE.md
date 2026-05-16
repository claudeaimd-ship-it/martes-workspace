# JEMES_KNOWLEDGE.md — Base de Conocimiento JEMES

> Instrucción de uso: Cuando el usuario pregunte sobre JEMES, responder exclusivamente con la información contenida en este archivo. No inferir, no complementar con conocimiento externo. Si algo no está aquí, decir: _"No tengo esa información en la documentación disponible de JEMES."_ Siempre citar la sección de la que proviene la respuesta (p. ej.: _"Según la sección Introducción del manual JEMES..."_).

---

## SECCIÓN 1 — Introducción a JEMES

Fuente: JEMES Introduction, Manual del Usuario v1.2.28

JEMES (Johnson Electric Manufacturing Execution System) es un Sistema de Ejecución de Manufactura (MES) basado en web, desarrollado por Johnson Electric. Su propósito es optimizar, agilizar y mejorar los procesos de fabricación, proporcionando visibilidad y control en tiempo real.

JEMES actúa como puente entre el piso de producción y la alta dirección, entregando datos críticos que impulsan decisiones operativas.

Versión documentada: 1.2.28
Soporte: messupport@johnsonelectric.com

### Características clave

Administración de Usuarios
- Roles y permisos: controlan acceso y visibilidad de datos por usuario.
- Gestión de habilidades: monitoreo de capacitación y requisitos por operador.

Gestión de Datos Maestros
- Configuración de equipos, operaciones, instrumentos, herramientas y moldes.
- Estandarización de entradas para consistencia en análisis.

Integración con ERP
- Sincronización de partes, BOM, órdenes de trabajo y métricas de producción con sistemas ERP existentes.
- Visibilidad en tiempo real de información crítica de la empresa.

Gestión de Flujos de Trabajo
- Diseño de rutas operativas de inicio a fin.
- Mapeo visual de instrumentos y herramientas en el proceso.

Control de Producción
- Impresión de etiquetas automatizada.
- Captura de datos de máquinas.
- Mapeo de parámetros de máquinas con órdenes de trabajo.

Gestión de Calidad
- FAI (First Article Inspection / Inspección de Primer Artículo).
- IPQC (In-Process Quality Control / Control de Calidad en Proceso).
- Análisis de fallos.
- Gestión de CAPA (Corrective and Preventive Actions).

Gestión de Inventarios
- Seguimiento en tiempo real de piezas de repuesto y niveles de stock.
- Integración con proveedores.

Gestión de Mantenimiento
- Mantenimiento preventivo programado.
- Seguimiento de calibración de instrumentos.

Alertas y Notificaciones
- Alertas configurables para calidad, producción y mantenimiento.
- Notificaciones en tiempo real para interrupciones críticas.

### Beneficios
- Mayor eficiencia operativa.
- Mayor precisión de datos (reducción de error humano).
- Reducción de costos operativos.
- Escalabilidad según el tamaño de la organización.

### Pasos iniciales para usar JEMES
1. Instalar la aplicación desde la fuente designada.
2. Crear cuentas de usuario y configurar roles.
3. Definir datos maestros (equipos, flujos de trabajo).
4. Conectar JEMES con el sistema ERP.
5. Capacitar a los usuarios en las funcionalidades.

---

## SECCIÓN 2 — Login

Fuente: Login, Manual del Usuario v1.2.28

Para acceder a JEMES:

1. Abrir el navegador web preferido (Chrome, Firefox, Safari).
2. Ingresar la URL proporcionada por el administrador en la barra de direcciones.
 - La pantalla inicial muestra el formulario de acceso con campos de usuario y contraseña. Hay un fondo con branding Johnson Electric y el logo de JEMES visible en la parte superior.
3. Introducir el nombre de usuario asignado.
4. Introducir la contraseña.
 - La pantalla de ingreso de contraseña muestra el campo de texto con opción de mostrar/ocultar la contraseña.
5. Hacer clic en "Iniciar Sesión".

Si las credenciales son correctas, el sistema redirige a la Página Principal de JEMES, que muestra el dashboard con el menú lateral de navegación y los módulos disponibles según el rol del usuario.

---

## SECCIÓN 3 — Administración de Usuarios

Fuente: Administration > User Administration, Manual del Usuario v1.2.28

### 3.1 Roles

La Página de Roles permite alos administradores definir y gestionar los roles de usuario, controlando qué páginas y módulos puede ver cada rol.

Acceso: Desde el menú lateral → opción "Roles", o desde la página de inicio.

La pantalla de Roles muestra una lista de roles existentes con botones de acción (Editar, Eliminar, Copiar) en cada fila, y un botón "Agregar" en la esquina superior derecha.

Operaciones disponibles:

- Agregar Rol: Clic en botón "Agregar" (esquina superior derecha) → completar detalles → clic en "Agregar" para guardar.
 - El formulario de guardado de rol muestra campos de nombre y descripción del rol.
- Editar Rol: Seleccionar el rol de la lista → clic en botón "Editar" → realizar cambios → guardar.
 - El botón de edición aparece como ícono de lápiz en cada fila de la lista.
- Eliminar Rol: Clic en ícono de eliminar → confirmar.
- Copiar Rol: Duplicar un rol existente para modificarlo como base de uno nuevo.
- Autorización de Rol: Clic en "Autorización de Rol" → seleccionar rol → habilitar/deshabilitar acceso a pantallas específicas → guardar.
 - La pantalla de Autorización muestra una lista de módulos con checkboxes que se pueden activar o desactivar por rol.

### 3.2 Skill (Habilidades)

Módulo para registrar y monitorear las habilidades de los operadores y sus requisitos de capacitación.

### 3.3 User Admin

Gestión de cuentas de usuario, asignación de roles y control de acceso individualizado.

### 3.4 View User Access

Vista consolidada de los permisos actuales de todos los usuarios.

### 3.5 Localization

Configuración de idioma y región del sistema.

### 3.6 Notification Management

Configuración de alertas y notificaciones por módulo y por usuario.

### 3.7 Page Rotater Management

Administración de rotación automática de pantallas (útil para dashboards en planta).

---

## SECCIÓN 4 — Ejecución: Production Operator Console (POC)

Fuente: Execution > Production Operator Console, Manual del Usuario v1.2.28

La Consola del Operador de Producción (POC) es la interfaz principal del operador en piso. Conecta al operador con el MES en tiempo real.

### Funciones principales
- Gestión de Órdenes de Trabajo: Ver, iniciar, pausar o completar órdenes asignadas.
- Gestión de Materiales: Solicitar, emitir y devolver materias primas.
- Actualizaciones de Estado: Marcar trabajos como en progreso, completados o en espera.
- Reporte de Chatarra: Registrar materiales defectuosos.
- Controles de Calidad: Registrar inspecciones durante la producción.
- Entrada de Datos: Capturar cantidades producidas, rendimiento de máquinas, razones de paro.
- Flujos Guiados: Mostrar instrucciones, dibujos y documentos al operador.
- Alertas: Escasez de material, averías de equipo.

### Cómo acceder
1. Navegar en el menú lateral → "Consola del Operador de Producción".
2. Seleccionar: Empresa → Planta → Área → Línea (en ese orden, o seleccionar directamente la Línea y el resto se autocompleta).
3. Se muestra la pantalla con: Número de Orden de Trabajo, Estado, Número de Parte, Cantidad Planificada y más.

### Solicitud de Material
1. Clic en "Solicitar Material" (esquina superior derecha de la POC).
2. Seleccionar Línea.
3. Seleccionar Orden de Trabajo.
4. Seleccionar las partes de Materia Prima necesarias (checkbox en columna "Acción").
5. Clic en "Enviar". Mensaje de confirmación: _"Material solicitado con éxito."_

Para ver historial de solicitudes anteriores: botón "Solicitudes Previas".

---

## SECCIÓN 5 — Detalles Técnicos: Mensajes MQTT

Fuente: Technical Details > MQTT Messages, Manual del Usuario v1.2.28

JEMES recibe datos de los equipos de planta mediante el protocolo MQTT.

### 5.1 Mensaje de Estado de Unidad (Unit Status)

Dirección: Equipo → JEMES
Protocolo: MQTT
Condición de envío: Solo si la unidad tiene número de serie.
Retroalimentación: No requiere respuesta.

Importante: El mensaje debe enviarse tan pronto como la unidad termine la prueba. Un envío retrasado o por lotes afecta el cálculo de OEE de la estación.

**Estructura del tema MQTT:**
/UnitStatus/{NombreLinea}
Ejemplo para línea H01: /UnitStatus/H01

QoS recomendado: Nivel 1 (al menos una vez).

Campos del mensaje JSON:

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Empresa | string | Nombre de la empresa (ej. "Johnson Electric") |
| Planta | string | Nombre de la planta (ej. "KM") |
| Área | string | Área dentro de la planta (ej. "Ensamblaje") |
| Línea | string | Nombre de la línea (ej. "H01") |
| MarcaDeTiempo | string ISO 8601 | Timestamp de generación del mensaje |
| NúmeroDeActivo | string | ID del equipo (ej. "B98765") |
| NúmSerie | string | Número de serie de la unidad |
| NúmSerieCliente | string | Número de serie del cliente para trazabilidad |
| CódigoEstado | integer | Estado actual de la unidad (debe existir en JEMES) |
| EquipoActual | string | Estación actual (ej. "Eq1") |
| SiguienteEquipo | string | Próxima estación (ej. "Eq2") |
| NúmeroDeEjecución | integer | Conteo de ejecuciones |
| ProductoTerminado | boolean | true = es producto terminado |
| EstadoUnidad | boolean | true = aprobó, false = falló |
| NombreProyecto | string | Nombre del proyecto (ej. "5YY0935") |
| CódigoTipo | integer | Tipo de estado (0 = predeterminado) |
| NúmeroDePalet | integer | Número de palet |
| CódigoHerramienta | string | Código de la herramienta usada |
| TipoParte | integer | Código del tipo de parte |
| SerialAdicional | array | Seriales adicionales relacionados a la unidad |
| Proceso | array | Parámetros de proceso: NombreProceso, ValorProceso, TipoProceso |

TipoProceso: 1 = Entero, 2 = Cadena, 3 = Decimal.

Ejemplo de payload JSON:
{
 "Empresa": "Johnson Electric",
 "Planta": "KM",
 "Área": "Ensamblaje",
 "Línea": "H01",
 "MarcaDeTiempo": "2024-09-18T10:00:00Z",
 "NúmeroDeActivo": "B98765",
 "NúmSerie": "ABC",
 "EstadoUnidad": true,
 "ProductoTerminado": true,
 "Proceso": [
 {"NombreProceso": "Voltaje-V", "ValorProceso": "13.000", "TipoProceso": 1}
 ]
}

### 5.2 Otros mensajes MQTT disponibles
- Equipment Heartbeat: Señal periódica de vida del equipo.
- Equipment Downtime: Reporta paros del equipo.
- Equipment OEE: Envía datos para cálculo de OEE.
- Equipment Process Parameters: Actualiza parámetros de proceso.
- Equipment Update Production: Actualiza estado de producción.

---

## SECCIÓN 6 — Endpoints de Hardware Compatibles

Fuente: Endpoints Hardware, Manual del Usuario v1.2.28

### Dispositivos PDA

Datalogic Skorpio X5
- Fabricante: Datalogic
- Modelo: Skorpio X5
- Dispositivo de mano tipo pistola con lector de códigos de barras integrado, pantalla táctil y teclado físico. Diseñado para entornos industriales.

Zebra TC22
- Fabricante: Zebra
- Modelo: TC22
- Dispositivo tipo smartphone industrial con lector de barras/QR integrado. Más compacto que el Skorpio, orientado a uso en piso de producción.

### Impresoras

TSC MH361
- Fabricante: TSC
- Modelo: MH361
- Impresora de etiquetas industrial de transferencia térmica. Formato medio-grande para etiquetas de producción.

SATO CL4NX Plus -C
- Fabricante: SATO
- Modelo: CL4NX Plus -C
- Impresora de etiquetas industrial de alta velocidad y precisión. Compatible con múltiples protocolos de comunicación.

---

## SECCIÓN 7 — Creación de Tickets de Soporte

Fuente: Support Ticket Creation, Manual del Usuario v1.2.28

Un ticket de soporte es una solicitud formal para reportar un problema, solicitar ayuda técnica o pedir aclaración sobre el sistema JEMES.

### Por qué son importantes
- Rastreo sistemático de problemas.
- Garantizan responsabilidad y resolución oportuna.
- Proveen historial para análisis.
- Evitan que problemas técnicos detengan la producción.

### Proceso para crear un ticket
1. Acceder al portal: http://sd.johnsonelectric.com/CAisd/pdmweb.exe
2. Iniciar sesión.
3. Clic en "Create a New Incident".
 - La pantalla muestra un formulario de incidente con campos secuenciales.
4. Ingresar correo electrónico (para recibir actualizaciones automáticas del ticket).
5. Ingresar número de móvil.
6.Ingresar número de dispositivo.
7. Ingresar información de ubicación.
8. En el campo "Incident Description", comenzar con el prefijo "JEMES" obligatoriamente.
 - ⚠️ Sin ese prefijo, el ticket no se considera relacionado con JEMES.
9. Agregar descripción detallada del problema.
10. Clic en "Save".
11. Guardar el número de referencia del ticket para seguimiento.

Correo de soporte directo: messupport@johnsonelectric.com

---

## SECCIÓN 8 — JEMES Data Warehouse

Fuente: JEMES Data Warehouse, Manual del Usuario v1.2.28

Arquitectura de exportación de datos desde JEMES hacia la nube para reportes en Power BI.

Flujo general: Extracción → Staging → Procesamiento → Carga → Archivado

La arquitectura es común para todos los sitios de JEMES a nivel global.

### Componentes

Base de datos JEMES (MSSQL on-prem)
Contiene la tabla de control MST_CloudSettings con las siguientes columnas clave:

| Columna | Descripción |
|---------|-------------|
| Table_Name | Nombre de la tabla con schema |
| Table_Type | Master o Transactional |
| Last_ID | Último ID procesado (actualizado por el servicio Python) |
| ID_Column_Name | Nombre de la columna clave primaria |
| Records | Registros por archivo Parquet |
| Frequency_Mins | Intervalo de procesamiento (Master: cada 24h; Transaccional: cada 15 min) |
| Last_ProcessedDate | Última fecha procesada |
| Active_Columns | Columna de borrado lógico |

Stored Procedures disponibles:

| Procedimiento | Función |
|---------------|---------|
| UpdateCloudSettingsLastID | Actualiza el último ID procesado |
| UpdateCloudSettingsLastProcessedTime | Actualiza fecha/hora de último procesamiento |
| GetCloudSettingsCurrentDateTime | Retorna datetime actual de la BD |
| CloudCheckProcessFrequency | Evalúa si la tabla debe procesarse (retorna boolean) |
| GetCloudHeader | Retorna el Site ID |
| GetCloudSettings | Retorna todas las filas de MST_CloudSettings |

Servicio Python (Windows Service)
Se ejecuta periódicamente. Lee desde JEMES, escribe archivos Parquet en Azure Blob Storage y actualiza MST_CloudSettings.
La estructura de carpetas en Azure Blob sigue un esquema jerárquico por sitio/tabla/fecha.
El archivo de configuración contiene: destinatarios de email, configuración de blob, credenciales de BD.

Carga en Synapse:
- Tablas Master: El target en Synapse se reemplaza completamente (reload).
- Tablas Transaccionales: Se agregan (append) nuevas filas al target.

Archivado en ADLS:
Después de cargar en Synapse con validación exitosa, los archivos Parquet se mueven a Azure Data Lake Storage para retención a largo plazo.

---

## SECCIÓN 9 — Módulos de Administración Adicionales

Fuente: Administration, Manual del Usuario v1.2.28

El menú de Administración incluye los siguientes módulos (documentación detallada disponible en el manual completo):

- MES Master: Configuración de datos maestros del sistema MES.
- ERP Master: Gestión de partes, BOM y configuración de integración ERP.
- Assets: Jerarquía de planta (Plant Hierarchy) — empresa, planta, área, línea.
- ERP Interface: Configuración de la interfaz entre JEMES y ERP.
- Workflow Manager: Diseño y gestión de flujos de trabajo de producción.
- Production: Secuencias de órdenes de trabajo.
- Maintenance Console: Alertas de averías y consola de mantenimiento.
- Quality: Consola PEA (Process Engineering Analysis).
- Warehouse: Gestión de almacén.
- Dashboard > Mini Andon: Dashboard de producción en tiempo real tipo Andon.

---

## NOTAS DE USO

- Este conocimiento corresponde a la versión 1.2.28 de JEMES.
- Para funcionalidades no documentadas aquí, referir al usuario al soporte oficial: messupport@johnsonelectric.com
- Las capturas de pantalla mencionadas en el manual original han sido convertidas a descripciones textuales en este documento para su uso sin imágenes.
