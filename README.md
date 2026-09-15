# El Comercio (Perú) — Prototipo con Plugin de Accesibilidad Cognitiva

Prototipo interactivo y accesible de un artículo periodístico del diario **El Comercio** (Perú), integrado con un sistema de **Accesibilidad Cognitiva** diseñado especialmente para lectores entre 35 y 70 años con TDAH, dislexia y fatiga atencional.

---

## 🌟 Características Principales

### 1. Cobertura Periodística Real
- **6 Secciones Informativas Reales y Conmutables**:
  - **Política**: Debate en el Hemiciclo sobre la reforma del sistema previsional con observaciones del MEF y la SBS.
  - **Lima**: Avance subterráneo de la tuneladora Micaela y pruebas de la Línea 2 del Metro de Lima.
  - **Economía**: Decisión de política monetaria del BCRP (tasa de 5.25%) y perspectivas del PBI.
  - **Opinión**: Editorial sobre productividad, seguridad jurídica y reformas estructurales.
  - **Mundo**: Cumbre Asia-Pacífico (APEC) sobre transición energética y libre comercio.
  - **Deporte Total**: Entrenamientos de la Selección Peruana en la Videna para la fecha doble de Eliminatorias.
- **Fotoperiodismo Real en Alta Definición**: Imágenes documentales auténticas con créditos editoriales.
- **Señal de Video en Directo**: Reproductor interactivo con controles de emisión, pausa y audio.
- **Publicidad Contextual Peruana**: Espacios publicitarios reales (BCP Cuenta Sueldo, Entel 5G, BBVA Ahorros, Interbank, Claro).

### 2. Modos de Asistencia Cognitiva (Heurísticas Nielsen & WCAG 2.2 AA)
- **Barra Superior de Estado Permanente**: Informa con claridad qué modo está activo y cuenta con botón de retorno inmediato (*"Volver al original ↺"* o *"Salir ↺"*).
- **Texto Adaptativo (Asistente IA Local Simulado)**:
  - *Los 4 Puntos Clave*: Jerarquía visual numerada y clara ideal para personas con TDAH.
  - *Resumen Express en 45 segundos*: Síntesis rápida para fatiga atencional.
  - *Lenguaje Sencillo*: Explicación en vocabulario cotidiano libre de tecnicismos complejos.
- **Interfaz Limpia (Modo Concentración)**:
  - Pone en negro los anuncios publicitarios y apaga las transmisiones de video, eliminando estímulos visuales y parpadeos.
  - Deja únicamente el texto del artículo para una lectura concentrada y sin distracciones.
- **Máscara de Lectura (Focus Mask)**:
  - Atenúa los párrafos circundantes y resalta el párrafo activo.
  - Navegación mediante flechas del teclado (↑ y ↓) o controles en pantalla con contador de progreso (ej. `1/6`).
- **Glosario Cognitivo Interactivo**:
  - Términos especializados (*sistema previsional*, *modelo multipilar*, *SBS*, *MEF*, *BCRP*, *APEC*, *Videna*, etc.) identificados con subrayado accesible.
  - Modal explicativo con lectura por voz y lenguaje claro.

### 3. Síntesis de Voz Inteligente (Web Speech API)
- Lectura completa del artículo, resúmenes de IA o párrafos individuales.
- Barra reproductora flotante con pausa, reanudación y detención.
- Calibración de ritmo de lectura (0.8x a 1.3x) con prueba auditiva previa.

### 4. Perfil y Personalización Tipográfica
- Tipografías especializadas: **OpenDyslexic**, **Atkinson Hyperlegible** y familia Serif.
- Calibración del tamaño de fuente (16px a 26px).
- Paletas de contraste accesible: **Neutro**, **Sepia cálido**, **Frío descansado** y **Noche oscura**.

### 5. Servicios Institucionales Simulados (Client-Side)
- **Club El Comercio**: Visualización de tarjeta de socio virtual con código QR y catálogo de beneficios en gastronomía, cines, viajes y salud.
- **Suscríbete**: Pasarela simulada con planes Digital y Total, selección de medio de pago y confirmación inmediata.
- **Iniciar Sesión**: Autenticación simulada con acceso rápido (Google / Apple) o formulario con validación de correo, actualizando el perfil de usuario en la cabecera.

---

## 🚀 Instalación y Ejecución Local

Este proyecto está construido con **HTML5, Tailwind CSS y TypeScript/Vite**, compatible directamente con cualquier servidor web o plataforma como GitHub Pages, Vercel, Netlify o Cloud Run.

```bash
# 1. Clonar el repositorio
git clone <URL_DEL_REPOSITORIO>
cd <CARPETA_DEL_PROYECTO>

# 2. Instalar dependencias
npm install

# 3. Iniciar servidor de desarrollo
npm run dev

# 4. Construir para producción (genera la carpeta dist/)
npm run build
```

El servidor local se iniciará en `http://localhost:3000`.

---

## ♿ Estándares de Accesibilidad Implementados

1. **Visibilidad del Estado del Sistema (Nielsen 1)**: Barra de notificación superior permanente en color negro con indicador del modo activo.
2. **Control y Libertad del Usuario (Nielsen 3)**: Botones visibles de cierre (✕), escape con tecla `Esc` y restablecimiento total de parámetros.
3. **Reconocer antes que Recordar (Nielsen 6)**: Controles con previsualización en tiempo real y glosario en el punto de lectura.
4. **WCAG 2.2 Nivel AA**:
   - Contraste superior a 4.5:1 en todos los textos y temas.
   - Tamaños táctiles mínimos de 44x44 px (`min-touch`).
   - Sin animaciones automáticas intrusivas ni parpadeos.
   - Compatibilidad total con teclado y lectores de pantalla.

---

## 📄 Licencia

Desarrollado como prototipo funcional de accesibilidad web para **El Comercio** (Perú).
