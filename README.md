# ✦ La Mágica Bruja Efsun

> Sitio web completo para un negocio de servicios esotéricos — tienda online, reservas, blog y horóscopo generado por inteligencia artificial.

![HTML](https://img.shields.io/badge/HTML-vanilla-e6cc72?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-vanilla-a482dc?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-c8a448?style=flat-square&logo=javascript&logoColor=white)
![IA](https://img.shields.io/badge/IA-Claude%20Sonnet-6e52b0?style=flat-square)
![Deploy](https://img.shields.io/badge/deploy-static%20hosting-52b882?style=flat-square)

---

## 🔮 Demo

Aplicación de página única — abre `index.html` directamente en el navegador, sin servidor ni dependencias.

---

## ✨ Funcionalidades

### Horóscopo con IA
Lecturas personalizadas generadas en tiempo real por Claude (Anthropic). El usuario selecciona su signo zodiacal, introduce su fecha de nacimiento y elige el área de consulta (amor, trabajo, salud o consejo del día). La respuesta aparece con efecto de escritura progresiva, como si el oráculo hablara en vivo.

### Sistema de reservas (4 pasos)
Flujo guiado para agendar sesiones presenciales u online: selección de servicio y modalidad → calendario con horarios disponibles → datos del cliente → pago seguro (tarjeta, PayPal o Bizum). Incluye resumen lateral en tiempo real y pantalla de confirmación con número de referencia.

### Tienda online
20 productos esotéricos organizados en 9 categorías (velas rituales, cristales, baños energéticos, tarot, amuletos, inciensos, aceites esenciales y libros). Carrito lateral con gestión de cantidades, aviso de envío gratis a partir de 60 € y envío a España y Europa.

### Catálogo de servicios
6 servicios detallados con descripción, modalidad disponible (presencial / online), duración y precio. Botón de reserva directo integrado en cada tarjeta.

### Blog esotérico
5 artículos completos sobre luna, astrología, tarot y rituales. Incluye sistema de comentarios con valoración por estrellas, productos relacionados vinculados a cada artículo y filtro por categorías.

### Extras
- Cursor personalizado de escoba mágica con partículas al hacer clic
- Fondo con nebulosas animadas y campo de estrellas multicapa
- Botón flotante de WhatsApp con enlace directo
- Accesos directos a TikTok e Instagram desde el hero y el footer
- Diseño completamente responsive

---

## 🛠 Tecnología

| Capa | Detalle |
|------|---------|
| Frontend | HTML + CSS + JavaScript vanilla |
| IA | Claude Sonnet 4 (Anthropic API) |
| Build | Sin dependencias — archivo único `index.html` |
| Deploy | Cualquier hosting estático (GitHub Pages, Netlify, Vercel…) |

No hay frameworks, no hay `npm install`, no hay bundlers. Todo el código vive en un único archivo HTML autocontenido.

---

## 📁 Estructura

```
pyme-efsun/
├── index.html       # Aplicación completa (HTML + CSS + JS + imagen embebida)
└── README.md
```

---

## 🚀 Uso local

```bash
# Clona el repositorio
git clone https://github.com/tu-usuario/pyme-efsun.git
cd pyme-efsun

# Abre en el navegador (macOS)
open index.html

# Abre en el navegador (Linux)
xdg-open index.html

# Abre en el navegador (Windows)
start index.html
```

---

## 🌙 Horóscopo con IA — configuración

La sección de horóscopo llama directamente a la API de Anthropic desde el navegador. Para producción se recomienda mover esta llamada a un backend o proxy para no exponer la clave.

1. Obtén una API key en [console.anthropic.com](https://console.anthropic.com/)
2. En `index.html`, localiza la función `generateHoro()` y añade tu clave en la cabecera de la petición:

```js
headers: {
  'Content-Type': 'application/json',
  'x-api-key': 'TU_API_KEY_AQUI',
  'anthropic-version': '2023-06-01',
  'anthropic-dangerous-direct-browser-access': 'true'
}
```

> ⚠️ Nunca expongas una API key real en un repositorio público. Usa variables de entorno o un proxy en producción.

---

## 💼 Servicios disponibles

| Servicio | Duración | Precio |
|----------|----------|--------|
| Tarot | 60 min | 65 € |
| Videncia | 60 min | 75 € |
| Limpia energética | 60 min | 55 € |
| Ritual personalizado | 90 min | 95 € |
| Trabajo de magia | 90 min | 110 € |
| Consulta de pareja | 75 min | 85 € |

---

## 🛍 Categorías de la tienda

Velas rituales · Cristales y piedras · Baños energéticos · Mazos de tarot · Amuletos y talismanes · Inciensos y resinas · Aceites esenciales · Libros y guías

---

## 📱 Redes sociales

| Red | Enlace |
|-----|--------|
| TikTok | [@brujaefsun](https://www.tiktok.com/@brujaefsun) |
| Instagram | [@lamagica.bruja.efsun](https://www.instagram.com/lamagica.bruja.efsun) |
| WhatsApp | [+34 672 894 842](https://wa.me/34672894842) |

---

## 🧑‍💻 Créditos

Diseño y desarrollo web por [Melina Rivera](https://melinarivera.github.io)

---

*Desarrollado con amor y magia ✦*