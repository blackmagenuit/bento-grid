# 🎨 Bento Grid - Social Media AI Dashboard

Una solución moderna y responsive del [desafío Bento Grid de Frontend Mentor](https://www.frontendmentor.io/challenges/bento-grid-RMydElrlOj), implementando un dashboard para una plataforma de gestión de redes sociales con IA.

![Preview del proyecto](./design/desktop-design.jpg)

## 📋 Tabla de contenidos

- [Sobre el proyecto](#-sobre-el-proyecto)
- [Características](#-características)
- [Tecnologías](#-tecnologías)
- [Instalación](#-instalación)
- [Lo que aprendí](#-lo-que-aprendí)
- [Desafíos superados](#-desafíos-superados)
- [Autor](#-autor)

## 🚀 Sobre el proyecto

Este proyecto es un dashboard interactivo que muestra las capacidades de una plataforma de gestión de redes sociales potenciada por IA. El diseño utiliza un layout "bento grid" moderno con tarjetas de diferentes tamaños que se adaptan perfectamente a diferentes dispositivos.

### El desafío

- ✅ Crear un layout bento grid responsive con tarjetas de diferentes dimensiones
- ✅ Mantener la coherencia visual en desktop y móvil
- ✅ Implementar un diseño mobile-first
- ✅ Seguir fielmente la guía de estilo proporcionada

## ✨ Características

- 📱 **Totalmente responsive** - Se adapta perfectamente desde móvil hasta desktop
- 🎨 **Diseño bento moderno** - Grid con tarjetas de diferentes tamaños
- 🎯 **Código limpio** - HTML semántico y CSS organizado con custom properties
- 🚀 **Performance optimizado** - Imágenes WebP y fuentes optimizadas
- ♿ **Accesible** - Estructura semántica y textos alternativos

## 🛠 Tecnologías

- **HTML5** - Estructura semántica
- **CSS3** - Grid, Flexbox, Custom Properties
- **Google Fonts** - DM Sans (400, 500, 700)
- **Mobile-First** - Diseño responsive desde móvil

## 📦 Instalación

1. Clona el repositorio:
```bash
git clone https://github.com/blackmagenuit/bento-grid-main.git
```

2. Abre el proyecto:
```bash
cd bento-grid-main
```

3. Abre `index.html` en tu navegador favorito o usa un servidor local:
```bash
# Con Python
python -m http.server 8000

# Con Node.js (npx)
npx serve
```

4. Visita `http://localhost:8000` en tu navegador

## 💡 Lo que aprendí

### CSS Grid avanzado

Dominar CSS Grid para layouts complejos fue el principal aprendizaje. Implementé un sistema donde las tarjetas ocupan diferentes espacios:

```css
.bento-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 2rem;
}

/* Tarjeta principal ocupa 2x2 */
.card-main {
  grid-column: 2 / 4;
  grid-row: 1 / 3;
}

/* Tarjeta alta ocupa 2 filas */
.card-create {
  grid-column: 1 / 2;
  grid-row: 1 / 3;
}
```

### Diseño Mobile-First

Empezar con una sola columna y expandir a grid complejo:

```css
/* Base móvil */
.bento-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
}

/* Desktop */
@media (min-width: 768px) {
  .bento-grid {
    grid-template-columns: repeat(4, 1fr);
  }
}
```

### Custom Properties para temas consistentes

```css
:root {
  --purple-100: hsl(254, 88%, 90%);
  --purple-500: hsl(256, 67%, 59%);
  --yellow-500: hsl(39, 100%, 71%);
  --font-family: 'DM Sans', sans-serif;
}
```

## 🎯 Desafíos superados

1. **Balance visual**: Lograr que tarjetas de diferentes tamaños se vean armoniosas
2. **Contenido adaptable**: Ajustar imágenes y texto para que quepan en espacios variables
3. **Responsive perfecto**: Mantener la estética en todos los tamaños de pantalla
4. **Overflow control**: Manejar contenido que se desborda en tarjetas pequeñas

## 🔗 Links

- **Repositorio**: [GitHub](https://github.com/blackmagenuit/bento-grid)
- **Demo en vivo**: [GitHub Pages](https://blackmagenuit.github.io/bento-grid)
- **Perfil Frontend Mentor**: [@blackmagenuit](https://www.frontendmentor.io/profile/blackmagenuit)

## 👨‍💻 Autor

**blackmagenuit**

- GitHub: [@blackmagenuit](https://github.com/blackmagenuit)
- Frontend Mentor: [@blackmagenuit](https://www.frontendmentor.io/profile/blackmagenuit)

---

