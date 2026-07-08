# Progreso del proyecto

## 2026-06-22

### Objetivos
- Establecer un registro de progreso por sesión en el repositorio.
- Añadir un ejemplo claro para empezar a usarlo.

### Trabajo realizado
- Creado `progress.md` con formato de seguimiento.
- Actualizado `README.md` para documentar el uso del archivo de progreso.

### Próximos pasos
- Añadir una entrada nueva al final de cada sesión o día.
- Usar este registro para visualizar la progresión del desarrollo.

## 2026-06-24

### Objetivos
- Añadir un nuevo botón a la calculadora con función de raíz cuadrada (√).
- Mantener el diseño consistente de la cuadrícula de botones.
- Registrar el cambio en el archivo de progreso diario.

### Trabajo realizado
- Añadida nueva fila con botón **√ (Raíz cuadrada)** a la calculadora en la **segunda fila** (justo debajo de C).
- Implementada función `applySqrt()` que calcula la raíz cuadrada del número actual con manejo de errores.
- Añadidos tres botones vacíos para mantener la alineación visual de la cuadrícula (4 columnas).
- Implementado atajo de teclado **Shift+R** para activar la raíz cuadrada.
- Actualizado `index.html` con CSS para botones fantasma (`.empty-slot`) y manejadores de eventos.
- **Ajuste de posición:** Reposicionado el botón √ de la quinta fila a la segunda fila para mejor accesibilidad y coherencia visual.

### Cómo usar
- **Botón:** Introduce un número y haz clic en **√** para calcular su raíz cuadrada.
- **Teclado:** Introduce un número y presiona **Shift+R** para el mismo resultado.
- **Manejo de errores:** Si intentas calcular la raíz de un número negativo, se mostrará un mensaje de error.

### Próximos pasos
- Probar la funcionalidad con distintos valores (positivos, decimales, cero).
- Considerar otros botones útiles (potencia, porcentaje, inverso) en futuras sesiones.

## 2026-07-08

### Objetivos
- Añadir un nuevo botón **x²** (elevar al cuadrado) a la calculadora.
- Implementar atajo de teclado **Shift+2** para la función.
- Mantener consistencia visual con el resto de botones de operaciones.

### Trabajo realizado
- Agregado botón **x²** en la segunda fila (reemplazando uno de los `empty-slot` junto a √).
- Implementada función `applyPow2()` que calcula el cuadrado del número actual con manejo de errores.
- Conectado listener de click para el nuevo botón.
- Implementado atajo de teclado **Shift+2** utilizando `e.code === 'Digit2'` (detecta la tecla física, no el carácter).
- **Corrección importante:** Cambio de `e.key` a `e.code` para mayor compatibilidad con distintos layouts de teclado.

### Cómo usar
- **Botón:** Introduce un número y haz clic en **x²** para elevar al cuadrado.
- **Teclado:** Introduce un número y presiona **Shift+2** para el mismo resultado.
- **Ejemplo:** Ingresa `5` → `Shift+2` → Resultado: `25`

### Nota del Desarrollador
- Parece ser que el Shift+2 en el teclado númerico no se ha implementado

### Próximos pasos
- Considerar agregar más potencias (x³, x^n) si se requiere.
- Explorar otras funciones científicas (porcentaje, factorial, etc.).
