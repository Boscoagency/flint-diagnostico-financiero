# Diagnóstico de Madurez Financiera — Flint Consulting

Herramienta interactiva de autodiagnóstico que evalúa la madurez de la **dirección financiera** de una empresa a través de 20 preguntas distribuidas en 6 pilares. Al terminar, el usuario completa un formulario de contacto y recibe un reporte con su calificación, score por pilar, prioridades estratégicas y un llamado a la acción.

🔗 **Demo en vivo:** https://boscoagency.github.io/flint-diagnostico-financiero/

---

## ¿Qué incluye?

- **Diseño alineado a la marca Flint** — tipografía Playfair Display + Inter, botones tipo píldora, tarjetas e imágenes redondeadas, paleta cyan/negro.
- **Hero con imagen de fondo** y texto legible sobre overlay.
- **20 preguntas** en escala 1–5 agrupadas en 6 pilares: Control y Cumplimiento, Liquidez y Tesorería, Rentabilidad y Performance, Planeación y Presupuesto, Estructura de Capital, e Información y Decisiones.
- **Formulario de contacto** (compuerta previa al reporte) con:
  - Nombre, cargo, empresa, número de empleados (menú desplegable) y correo.
  - Validación de **correo empresarial** (rechaza Gmail, Hotmail, Outlook y otros dominios gratuitos).
  - Leyenda de la Ley Federal de Protección de Datos + enlace al Aviso de Privacidad.
  - Casillas de aceptación del Aviso de Privacidad (obligatoria) y de marketing (opcional).
- **Reporte automático** con score total (0–100), nivel de madurez, score por pilar, fortalezas y prioridades.
- **Envío por correo vía [Web3Forms](https://web3forms.com)** a `connect@flintconsulting.mx` con los datos del lead, el score y las 20 respuestas.

---

## Estructura

Es un único archivo autocontenido:

```
index.html        → todo el diagnóstico (HTML + CSS + JS en línea)
```

Las imágenes (hero) se cargan desde el CDN de Webflow de Flint, por lo que no se necesitan archivos adicionales. Puede usarse como página independiente o **embeberse** dentro del sitio (el menú y footer del sitio quedan fuera del componente).

---

## Configuración

- **Correo de destino / Web3Forms:** la `Access Key` está en `index.html`, en la constante `WEB3FORMS_ACCESS_KEY`. Está ligada a `connect@flintconsulting.mx`.
- **Aviso de Privacidad:** apunta a `https://www.flintconsulting.mx/legal/aviso-de-privacidad`.
- **Espaciador superior:** la clase CSS `.nav-spacer` reserva el espacio para el menú del sitio cuando se embebe (altura ajustable).

---

## Actualizar el sitio

```bash
git add -A && git commit -m "ajustes" && git push
```

GitHub Pages reconstruye el sitio automáticamente (1–2 min).

---

*Built by Bosco Growth Marketing para Flint Consulting.*
