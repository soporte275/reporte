# Widget Económico — PIB · Per Cápita · Índice IPAC
**Autor:** Armando D. Núñez Chung  
**Empresa:** AST System Computer Technology | RUC 8-844-2003 DV:55  
**Sitio:** [ast-pty.com](https://www.ast-pty.com)  
**Fecha:** Marzo 2026  

---

## Descripción

Widget HTML autocontenido que presenta el análisis económico de Panamá bajo el paquete de reformas liberales (Escuela Austriaca), con **4 pestañas interactivas**:

| Pestaña | Contenido |
|---|---|
| PIB 2015–2035 | Gráfico histórico + proyección base FMI vs. con reformas |
| PIB Per Cápita | Curva por ciudadano + referencia Chile |
| Índice IPAC | Nueva métrica de poder adquisitivo ciudadano (propuesta autoral original) |
| Simulador | 5 sliders de reforma con resultados en tiempo real |

---

## Instalación

### Opción A — Bloque HTML en Horizon / CMS
1. Abre `widget-economia-panama.html` en un editor de texto
2. Copia **todo** el contenido entre las marcas:
   ```
   <!-- ═══════════════════════ INICIO WIDGET ═══════════════════════ -->
   ...
   <!-- ════════════════════════ FIN WIDGET ════════════════════════ -->
   ```
3. En Horizon: **Agregar bloque → HTML personalizado** → pega el código → Guardar

### Opción B — iframe embebido
Sube el archivo a tu hosting y embébelo:
```html
<iframe src="/widget-economia-panama.html" 
        width="100%" height="750" 
        frameborder="0" style="border:none;">
</iframe>
```

### Opción C — Página independiente
Sirve directamente el archivo `.html` como ruta propia en tu servidor, por ejemplo:
```
https://www.ast-pty.com/economia
```

---

## Requisitos técnicos

- ✅ **Sin dependencias locales** — Chart.js 4.4.1 se carga automáticamente desde CDN
- ✅ **Sin frameworks** — HTML + CSS + JavaScript vanilla puro
- ✅ **CSS aislado** — todos los estilos usan el prefijo `#ast-eco-widget` para no interferir con el sitio
- ✅ **Responsive** — adaptado para móvil, tablet y escritorio
- ✅ **Carga lazy** — cada gráfico se inicializa solo cuando el usuario abre esa pestaña

---

## Índice IPAC — Propuesta Autoral Original

**IPAC = (Ingreso_mediano_real × (1 − Carga_fiscal_efectiva)) ÷ CPC_ajustada**

Donde `CPC_ajustada` = Costo Per Cápita de Vida Digna ajustado por PPP local.

Propuesta original de **Armando D. Núñez Chung**, basada en la crítica austriaca al PIB como métrica de bienestar (Mises). A diferencia del PIB per cápita, el IPAC mide el poder adquisitivo real del ciudadano del percentil 50.

---

## Fuentes de datos

- INEC Panamá — Encuesta de Mercado Laboral 2025
- MEF Panamá — Informe de Gestión Fiscal 2024
- Banco Mundial — WEO / WDI 2024–2025
- FMI — World Economic Outlook 2025
- CEPAL — Informalidad y carga laboral 2024
- Transparencia Internacional — IPC 2025

---

## Licencia y Propiedad Intelectual

© 2026 Armando D. Núñez Chung — AST System Computer Technology.  
Todos los derechos intelectuales reservados.  
El análisis, las métricas (especialmente el IPAC) y las proyecciones contenidas en este widget son propiedad intelectual del autor.  
Prohibida su reproducción parcial o total sin atribución expresa a **Armando D. Núñez Chung / AST System Computer Technology**.
