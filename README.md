# Accesorios García | Gestión Total Pro

Sistema completo de gestión de inventario para el negocio de accesorios "Accesorios García". Incluye dashboard administrativo, catálogo de productos para clientes, gestión de ventas, compras, pedidos, rifas, facturación, reportes y más.

## 🚀 Características Principales

### 📊 Dashboard Administrativo
- **Sidebar izquierdo** con navegación intuitiva a todas las secciones
- **Métricas en tiempo real**: Ventas totales, utilidad de rifas, pedidos pendientes, ganancia neta
- **Gráficos multicolores 3D** con efectos visuales avanzados
- **Escáner QR** integrado para productos (compatible con móviles y PC)

### 🛒 Gestión de Inventario
- **CRUD completo** para productos con categorías específicas:
  - Calzado de Dama/Caballero/Niño
  - Cañclas de Dama/Caballero/Niño
  - Mochilas de Cuero
  - Pulseras de Plata
- **Subida de fotos** de productos (almacenamiento base64)
- **Descripciones detalladas** para cada producto
- **Control de stock** automático
- **Códigos SKU** únicos

### 💰 Operaciones Empresariales
- **Ventas**: Registro de movimientos de entrada/salida
- **Compras**: Gestión de proveedores y costos
- **Pedidos**: Sistema completo con anticipos y saldos pendientes
- **Rifas**: Gestión de boletos y utilidades
- **Facturación**: Generación de facturas

### 📱 Catálogo para Clientes
- **Modo cliente** exclusivo (acceso vía enlace o QR)
- **Vista de catálogo** filtrada por categorías
- **Imágenes y descripciones** de productos
- **Precios y stock disponible** en tiempo real
- **Interfaz limpia** sin secciones administrativas

### 🔗 Compartir Catálogo
- **Generación automática** de enlaces y códigos QR
- **Copiado al portapapeles** del enlace
- **Acceso directo** para clientes sin login

### 📈 Reportes y Exportaciones
- **Gráficos interactivos** con Chart.js
- **Exportación a Excel** de ventas y pedidos
- **Generación de PDFs** de tickets y reportes
- **Imágenes PNG** de tickets para impresión

## 🛠️ Tecnologías Utilizadas

### Frontend
- **HTML5** con Tailwind CSS para diseño moderno
- **JavaScript** puro para lógica de negocio
- **Chart.js** para gráficos multicolores 3D
- **QRCode.js** para generación de códigos QR
- **Html5Qrcode** para escáner de códigos QR
- **jsPDF** y **html2canvas** para exportaciones

### Backend / Almacenamiento
- **Firebase Firestore** para persistencia de datos en la nube
- **LocalStorage** como respaldo offline
- **Base64** para almacenamiento de imágenes

### Librerías Externas
- **Tailwind CSS** (CDN) para estilos responsivos
- **Font Awesome** para iconos
- **XLSX** para exportación Excel
- **QRCode.js** para códigos QR

## 📁 Estructura del Proyecto

```
📦 Gestión de Inventario
├── 📄 index.html          # Archivo principal con toda la aplicación
├── 📄 README.md           # Este archivo
└── 📁 imagen/
    └── 📄 Logo.jpg        # Logo de la empresa
```

## 🚀 Instalación y Uso

### Requisitos Previos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexión a internet para Firebase (opcional, funciona offline)
- Cámara para escáner QR (opcional)

### Configuración Inicial
1. **Descarga los archivos** del proyecto
2. **Abre `index.html`** en tu navegador
3. **Credenciales de acceso**:
   - Usuario: `proveedor`, Contraseña: `garcia77`
   - Usuario: `administrador`, Contraseña: `admin2026`
   - Usuario: `encargado`, Contraseña: `ventas01`

### Configuración de Firebase (Opcional)
El proyecto incluye configuración de Firebase para persistencia en la nube. Para usar tu propia base de datos:

1. Crea un proyecto en [Firebase Console](https://console.firebase.google.com/)
2. Habilita Firestore Database
3. Actualiza las credenciales en `index.html` (líneas 25-35)

## 📖 Guía de Uso

### Para Administradores
1. **Login**: Usa las credenciales proporcionadas
2. **Agregar Productos**: Ve a "Productos" → Completa formulario con foto, descripción y categoría
3. **Registrar Ventas**: Usa el formulario principal o el modal "Ventas"
4. **Gestionar Pedidos**: CRUD completo en la sección "Pedidos"
5. **Ver Reportes**: Gráficos y exportaciones en "Reportes"

### Para Clientes
1. **Recibe el enlace** o escanea el QR del catálogo
2. **Navega categorías** para ver productos
3. **Visualiza detalles**: Fotos, descripciones, precios y stock

### Compartir Catálogo
1. Ve a "Enlace Catálogo" en la sidebar
2. **Copia el enlace** o **escanea el QR**
3. **Comparte** con clientes para acceso directo

## 🎨 Características de Diseño

### Efectos Visuales
- **Gradientes multicolores** en botones y gráficos
- **Animaciones suaves** en hover de botones y tarjetas
- **Transiciones fluidas** en modales y secciones
- **Efectos 3D** simulados en gráficos

### Interfaz Responsiva
- **Diseño mobile-first** con Tailwind CSS
- **Compatible** con teléfonos, tablets y PC
- **Sidebar colapsable** en móviles

### Tema Visual
- **Colores corporativos**: Gradientes rosados y azules
- **Tipografía moderna**: Poppins font
- **Efectos glassmorphism** en tarjetas

## 🔧 Funcionalidades Técnicas

### Gestión de Estado
- **Base de datos local** con sincronización a Firebase
- **Persistencia offline** con localStorage
- **Sincronización automática** al cargar la página

### Seguridad
- **Sistema de login** con usuarios y roles
- **Modo cliente** restringido (solo lectura)
- **Validación de formularios** en tiempo real

### Optimizaciones
- **Lazy loading** de imágenes
- **Compresión base64** para fotos de productos
- **Caché inteligente** de datos

## 📊 Estadísticas y Métricas

El dashboard muestra en tiempo real:
- **Ventas totales** acumuladas
- **Utilidad de rifas** (boletos vendidos - costo premio)
- **Pedidos pendientes** (total - anticipos pagados)
- **Ganancia neta** (ventas + rifas)

## 🐛 Solución de Problemas

### Firebase no conecta
- Verifica conexión a internet
- Revisa credenciales en el código
- Los datos se guardan localmente como respaldo

### Escáner QR no funciona
- Permite acceso a la cámara en el navegador
- Usa un dispositivo con cámara
- Fallback automático a entrada manual

### Imágenes no se muestran
- Verifica que el archivo `Logo.jpg` exista en `imagen/`
- Las fotos de productos se almacenan como base64

## 🚀 Próximas Mejoras

- [ ] Backend Python con Flask para mayor escalabilidad
- [ ] API REST para integraciones externas
- [ ] Notificaciones push para pedidos
- [ ] Sistema de usuarios avanzado
- [ ] Análisis predictivo de inventario
- [ ] Integración con WhatsApp para pedidos

## 📄 Licencia

Este proyecto es de uso privado para "Accesorios García". No distribuir sin autorización.

## 👥 Soporte

Para soporte técnico o modificaciones, contacta al desarrollador.

---

**Desarrollado con ❤️ para Accesorios García**
