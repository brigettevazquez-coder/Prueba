# 🎓 Tiendita Escolar - Recaudación de Fondos

Una aplicación web moderna para gestionar una tienda de recaudación de fondos escolares. Perfecta para vender productos y rastrear el progreso hacia tu meta de fondos.

## ✨ Características

✅ **Catálogo de productos** - Organizado por categorías (Comida, Artesanías, Ropa)
✅ **Carrito de compras** - Agregar, modificar y eliminar cantidades
✅ **Formulario de checkout** - Recolecta información del cliente
✅ **Persistencia de datos** - El carrito se guarda automáticamente
✅ **Historial de pedidos** - Todos los pedidos se almacenan localmente
✅ **Barra de progreso** - Visualiza el progreso hacia la meta
✅ **Diseño responsivo** - Funciona perfecto en móvil y desktop
✅ **Modo oscuro** - Soporte automático para tema oscuro
✅ **Sin dependencias** - Solo HTML, CSS y JavaScript vanilla

## 🚀 Cómo usar

### Opción 1: En línea (GitHub Pages)
Abre directamente en tu navegador:
```
https://brigettevazquez-coder.github.io/Prueba/
```

### Opción 2: Localmente
1. Descarga o clona el repositorio
2. Abre `index.html` en tu navegador
3. ¡Listo! La aplicación está lista para usar

## 📋 Instrucciones de uso

### 1. Navegar productos
- Usa los botones de filtro para ver productos por categoría
- Cada producto muestra nombre, descripción y precio

### 2. Agregar al carrito
- Haz clic en el botón `+` verde para agregar un producto
- El carrito se actualiza automáticamente
- Aparecerá el total a pagar

### 3. Ajustar cantidades
- Usa los botones `-` y `+` en el carrito para cambiar cantidades
- Elimina un producto reduciendo a cero

### 4. Confirmar pedido
1. Haz clic en **"✓ Confirmar pedido"**
2. Completa el formulario con:
   - Nombre (requerido)
   - Teléfono (requerido)
   - Email (requerido)
   - Notas (opcional)
3. Haz clic en **"✓ Confirmar"**
4. El pedido se guarda y suma a la meta

### 5. Vaciar carrito
- Haz clic en **"🗑️ Vaciar"** para limpiar el carrito
- Se pedirá confirmación antes de eliminar

## 💾 Datos guardados

Los datos se almacenan en tu navegador (localStorage):
- ✅ `tiendita_cart` - Tu carrito actual
- ✅ `tiendita_total` - Total recaudado
- ✅ `tiendita_orders` - Historial de todos los pedidos

**Para ver los datos guardados:**
1. Abre DevTools (`F12` o `Ctrl+Shift+I`)
2. Ve a **Application** → **Local Storage**
3. Busca las claves anteriores

## 🎨 Personalización

### Cambiar productos
Edita el array `products` en `index.html`:
```javascript
const products = [
  { 
    id: 1, 
    name: 'Tu producto',
    cat: 'Categoría',
    icon: '🎉',
    desc: 'Descripción del producto',
    price: 100,
    color: 'cat-comida'
  },
  // ... más productos
];
```

### Cambiar meta de recaudación
Busca `const goal = 5000;` y cambia el número

### Cambiar colores
Edita las variables CSS en la sección `:root`:
```css
:root {
  --green: #1a6b3c;  /* Color principal */
  --green-pale: #7fffc4;  /* Color de la barra de progreso */
  /* ... más colores */
}
```

## 📱 Compatibilidad

- ✅ Chrome/Edge/Firefox/Safari
- ✅ Móviles (iOS/Android)
- ✅ Tablets
- ✅ Modo oscuro automático

## 🛠️ Tecnologías

- HTML5
- CSS3 (con variables y media queries)
- JavaScript vanilla (sin frameworks)
- Icons: [Tabler Icons](https://tabler.io/icons)

## 📄 Productos incluidos

### Comida 🍞
- Tamales de pollo - $120
- Agua fresca de jamaica - $35
- Galletas decoradas - $80

### Artesanías 🎨
- Pulsera tejida - $45
- Maceta pintada - $90
- Tarjetas recicladas - $60

### Ropa 👕
- Playera de la escuela - $150
- Gorra bordada - $120

## 🎯 Meta

Meta de recaudación: **$5,000**
Grupo: **4°B**

## ⚠️ Notas importantes

- Los datos se guardan **localmente** en cada dispositivo
- Si limpias el caché del navegador, se perderán los datos
- Para sincronizar datos entre dispositivos, necesitarías un backend (servidor)
- Los pedidos NO se envían a email automáticamente (necesitaría un servidor)

## 🚀 Futuras mejoras

Posibles características:
- [ ] Integración con WhatsApp para enviar pedidos
- [ ] Envío de confirmación por email
- [ ] Dashboard administrativo para ver pedidos
- [ ] Sincronización en la nube
- [ ] Exportar datos a CSV
- [ ] Múltiples administradores

## 📞 Contacto

¿Preguntas o sugerencias? Abre un issue en GitHub

---

**Creado con ❤️ para recaudar fondos escolares**
