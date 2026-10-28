# ✈️ ZX TURISMO

> «Tu próxima aventura comienza aquí».

Plataforma turística **de demostración** hecha con HTML, CSS y JavaScript en un solo archivo (`index.html`). Simula una agencia de viajes internacional: destinos, vuelos, carrito, cuentas, facturas, boletos con QR y un asistente virtual llamado **ZUX AI**.

🔗 **Demo en vivo (GitHub Pages):** `https://TU-USUARIO.github.io/zx-turismo/` *(reemplaza TU-USUARIO por tu nombre de usuario de GitHub)*

> ⚠️ **Proyecto de demostración.** Los precios, vuelos, testimonios y estadísticas son ficticios. No se realizan cobros reales ni se piden datos de tarjeta. Los boletos y facturas no tienen validez fiscal ni sirven para viajar.

## 📁 Estructura

```
zx-turismo/
├── index.html                 # La página web completa (código, fotos y videos incrustados)
├── README.md                  # Este archivo
├── LICENSE                    # Licencia MIT (código)
├── .gitignore
├── .nojekyll                  # Desactiva Jekyll en GitHub Pages
└── docs/
    ├── MANUAL_DE_CALIDAD.md   # Manual de calidad del proyecto
    └── Informe_Manuales_de_Calidad_para_Paginas_Web.pdf   # Informe de referencia
```

## ✨ Funciones

- **34 destinos** con paquetes de 5 días, filtros por continente, búsqueda, orden por precio y favoritos.
- **Buscador de vuelos** (datos de demostración) con tres opciones por búsqueda.
- **Carrito persistente** (localStorage): cantidades, eliminar, cupones (`ZX10`, `BIENVENIDA100`), descuentos e IVA.
- **Cuentas de usuario**: registro, inicio de sesión (contraseña con hash SHA-256 y sal), cupón de bienvenida, favoritos.
- **Membresías** Premium ($99/año) y SUPER ZX ($499/año), con pago simulado.
- **Compra de demostración** con validación de formularios, **factura** y **boletos con código QR real** y página de verificación.
- **Galería**, carrusel automático, visor de fotos (lightbox) y **dos videos** (Nueva York y Río de Janeiro).
- **ZUX AI**: asistente virtual de demostración (motor de reglas en JavaScript, sin API externa). Entiende errores de ortografía comunes, recuerda el contexto (destino, personas, presupuesto), recomienda según presupuesto, compara destinos, explica cómo reservar y agrega paquetes al carrito **solo con tu confirmación**. Si no entiende, lo dice y ofrece alternativas.
- Modo claro/oscuro y diseño adaptable a móviles.

## 🚀 Cómo ejecutarlo

**Opción 1 — Local:** descarga el repositorio y abre `index.html` en tu navegador (Chrome, Edge, Firefox o Safari).

**Opción 2 — GitHub Pages:**
1. En el repositorio ve a **Settings → Pages**.
2. En *Build and deployment*, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
3. Guarda y espera uno o dos minutos. Tu página quedará en `https://TU-USUARIO.github.io/zx-turismo/`.

## 🧪 Calidad

El proyecto sigue el [Manual de calidad](docs/MANUAL_DE_CALIDAD.md), basado en ISO/IEC 25010, WCAG 2.2, Core Web Vitals y OWASP. Ahí están los criterios de aceptación y el estado real de cada verificación.

## 🔧 Qué falta para ser una plataforma comercial

| Pieza | Estado | Necesita |
|---|---|---|
| Pagos reales | Simulado | Pasarela de pago (Stripe, PayPal, etc.) y backend |
| Cuentas y base de datos | En el navegador (localStorage) | Backend con base de datos y autenticación segura |
| Vuelos y disponibilidad | Datos ficticios | API de aerolíneas/GDS |
| Verificación de QR | Solo en el mismo navegador | Servidor que consulte la reservación |
| ZUX AI generativa | Motor de reglas | API de un modelo de lenguaje con backend (la clave nunca va en el navegador) |
| Fotos de 12+ destinos | Ilustrativas (marcadas) | Fotografías propias o con licencia |
| Panel administrativo | No incluido | Backend y roles |

## 📸 Créditos

Fotografías y videos aportados por el autor del proyecto; verificar licencias y créditos antes de un uso comercial. Código QR generado con [qrcodejs](https://github.com/davidshimjs/qrcodejs).

## 📄 Licencia

Código bajo licencia [MIT](LICENSE).
