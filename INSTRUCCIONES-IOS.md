# 📱 Instrucciones para iOS - Recordatorios de Alquiler

## ✅ Cómo agregar la app a la pantalla de inicio de iOS

1. **Abrir Safari** en tu iPhone/iPad
2. **Navegar a la URL** de la app (ej: `http://localhost:8000` o tu URL desplegada)
3. **Tocar el botón "Compartir"** (cuadrado con flecha hacia arriba)
4. **Deslizar hacia abajo** y seleccionar **"Agregar a la pantalla de inicio"**
5. **Confirmar** con "Agregar"

## 🔔 Cómo habilitar las notificaciones

### Paso 1: Solicitar permisos
- Al abrir la app por primera vez, aparecerá un mensaje pidiendo permisos para notificaciones
- **Tocar "Permitir"** cuando aparezca el mensaje

### Paso 2: Verificar configuración
- Ir a **Configuración > Notificaciones** en tu iPhone
- Buscar **"Recordatorios de Alquiler"** o el nombre que le diste a la app
- Asegurarse de que esté **activado**:
  - Permitir notificaciones: ✅
  - Sonidos: ✅ (opcional)
  - Insignas: ✅ (opcional)
  - Mostrar en pantalla de bloqueo: ✅ (opcional)

## 📋 Cómo funciona el sistema de notificaciones

### Mensaje de notificación
Cuando llega el día de renovar un alquiler, recibirás una notificación con este formato exacto:

**Título:** `🏠 Renovación de Alquiler - [Nombre del Alquiler]`

**Mensaje:** `Hoy tenés que renovar este alquiler. Previamente cobraste $[monto anterior] y ahora actualizándolo tomando en cuenta la inflación del período tenés que cobrar $[monto actualizado]`

### Ejemplo real:
- **Título:** `🏠 Renovación de Alquiler - Terreno en el centro`
- **Mensaje:** `Hoy tenés que renovar este alquiler. Previamente cobraste $1.000.000 y ahora actualizándolo tomando en cuenta la inflación del período tenés que cobrar $1.270.000`

## 🔄 Frecuencia de notificaciones

- **Verificación automática:** Cada vez que abrís la app
- **Verificación periódica:** Cada hora mientras la app esté abierta
- **Evita duplicados:** Solo se envía una notificación por día por alquiler

## ⚙️ Configuración adicional

### Si no recibís notificaciones:
1. **Verificar permisos** en Configuración > Notificaciones
2. **Reiniciar la app** (cerrarla completamente y volver a abrir)
3. **Asegurarte de tener alquileres vencidos** (la fecha de actualización ya pasó)

### Para probar las notificaciones:
1. **Agregar un alquiler** con fecha de inicio de hace 3 meses
2. **Establecer frecuencia** de actualización en 3 meses
3. **Abrir la app** - deberías recibir la notificación inmediatamente

## 📊 Cálculo de inflación

La app utiliza datos de inflación trimestral de Argentina:
- **Tasa actual:** 8-13% por trimestre (ajustable)
- **Cálculo:** Monto actualizado = Monto base × (1 + tasa)^períodos
- **Redondeo:** A valores enteros en pesos argentinos

## 🆘 Solución de problemas

### No aparece la opción "Agregar a pantalla de inicio":
- **Usar Safari** (no funciona con Chrome u otros navegadores en iOS)
- **Asegurarse de estar en la página principal** (no en una subpágina)

### Las notificaciones no funcionan:
- **Verificar que las notificaciones estén activadas** en Configuración > Notificaciones
- **Permitir notificaciones** cuando la app lo solicite
- **Reiniciar el dispositivo** si es necesario

### El cálculo parece incorrecto:
- **Verificar la fecha de inicio** del alquiler
- **Revisar la frecuencia de actualización** configurada
- **Los montos se actualizan automáticamente** según la inflación del período
