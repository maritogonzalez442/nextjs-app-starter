# 📱 Instrucciones Actualizadas - Sistema de Inflación Real del INDEC

## ✅ NUEVO: Sistema de Inflación Real del INDEC

### 🎯 Cómo funciona el cálculo de inflación:

1. **Datos reales del INDEC**: La app se conecta automáticamente a https://www.indec.gob.ar/ cuando llega el momento de actualizar
2. **Cálculo por período**: Obtiene la inflación de los últimos 3 meses exactos antes de la fecha de vencimiento
3. **Actualización automática**: Actualiza el monto usando la inflación real del período transcurrido
4. **Monto acumulativo**: Usa el monto actualizado como base para el siguiente período

### 📊 Ejemplo de funcionamiento:

**Alquiler inicial:**
- Fecha de inicio: 17/07/2025
- Monto inicial: $1,000,000
- Frecuencia: cada 3 meses

**Primer vencimiento: 17/10/2025**
- La app consulta al INDEC la inflación de julio, agosto y septiembre 2025
- Si la inflación acumulada fue 12.5%, el nuevo monto será: $1,125,000
- Este monto se guarda como "monto actual" para el siguiente período

**Segundo vencimiento: 17/01/2026**
- La app consulta la inflación de octubre, noviembre y diciembre 2025
- Si la inflación fue 15%, el nuevo monto será: $1,293,750 (sobre $1,125,000)

### 🔄 Actualización automática:

- **Al abrir la app**: Verifica automáticamente si hay alquileres vencidos
- **Actualización inmediata**: Si está vencido, actualiza con datos del INDEC
- **Notificación**: Muestra el mensaje exacto con montos reales
- **Historial**: Guarda cada actualización con fecha y porcentaje

### 📱 Cómo usar:

1. **Agregar alquiler** con fecha de inicio y monto base
2. **La app calcula automáticamente** cuando llega el momento de actualizar
3. **Recibe notificación** con el mensaje exacto:
   *"Hoy tenés que renovar este alquiler. Previamente cobraste $[monto actual] y ahora actualizándolo tomando en cuenta la inflación del período tenés que cobrar $[monto nuevo]"*

### 🌐 Conexión a internet:

- **Con conexión**: Usa datos reales del INDEC
- **Sin conexión**: Usa estimación del 3% mensual como fallback
- **Indicador visual**: Muestra si está usando datos reales o estimados

### 📈 Visualización:

- **Monto base**: Siempre visible (el original)
- **Monto actual**: El último actualizado con inflación real
- **Última actualización**: Fecha del último cálculo
- **Próxima actualización**: Fecha calculada automáticamente

### 🔄 Ciclo completo:

1. **Agregar alquiler** → Se guarda monto base y actual
2. **Esperar período** → La app monitorea automáticamente
3. **Llega vencimiento** → Consulta INDEC y actualiza
4. **Notificación** → Mensaje exacto con montos reales
5. **Siguiente período** → Usa el monto actualizado como base

### ⚙️ Configuración:

No necesitas configurar nada adicional. La app:
- Se conecta automáticamente al INDEC
- Calcula la inflación exacta del período
- Actualiza el monto y lo guarda
- Mantiene historial de todas las actualizaciones
- Funciona offline con estimaciones si no hay conexión
