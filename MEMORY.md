# Memoria de Martes

## Reglas permanentes

- Incluir al final de CADA respuesta: `**API:** [modelo usado] — **Tokens:** [X]K in / [Y]K out`

## Historial de tokens

| Fecha | API | Tokens In | Tokens Out | Total |
|------|-----|----------|-----------|-------|
| 2026-05-16 | deepseek/deepseek-chat | — | — | — |

## Configuración de Base de Datos
- Servidor: MX01S201\SQLEXPRESS01
- Base de datos: Conteo_MiniAndon
- Estructura de tablas: NombreLinea_Maquina_Eol (cada fila = 1 pieza producida)
- Modo de acceso: Solo lectura

## Lógica de Negocio Confirmada
- Turno mañana: 07:00–14:59
- Turno tarde: 15:00–22:59
- Turno noche: 23:00–06:59 (cruza medianoche)
- Producción por hora = conteo de filas en el rango de tiempo de esa hora para la EOL
- Líneas identificadas por prefijo del nombre de tabla

## Decisiones Tomadas
| Fecha | Decisión |
|-------|----------|
| — | Cada fila en tablas EOL = una pieza producida |
| — | Solo lectura de datos |
| — | Formato de reporte: tabla hora×EOL + totales |
| 2026-05-16 | Telemetría: incluir API y tokens al final de cada respuesta |
| 2026-05-16 | Repositorio GitHub: martes-workspace subido |

## Líneas Conocidas
| Línea | Tablas Identificadas | Última Consulta |
|-------|----------------------|-----------------|
| Giotto | *(poblar en primera consulta real)* | — |

## Incidentes / Errores Registrados
*(vacío — se llena conforme ocurran)*

---
_Ver memory/ para registros diarios._
