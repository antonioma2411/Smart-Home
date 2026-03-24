# 🏠 SmartHome Dashboard: Control Residencial Inteligente

**SmartHome Dashboard** es una plataforma web estática de alto rendimiento diseñada para centralizar el control de dispositivos IoT (Internet of Things). El proyecto demuestra el uso de técnicas avanzadas de CSS moderno, como el manejo de estados visuales, diseño de tarjetas interactivas y una transición fluida entre modos de iluminación.

---

## 🚀 Vista Rápida

El objetivo de este proyecto es ofrecer una interfaz minimalista pero potente donde el usuario pueda monitorear:
* **Climatización:** Control de temperatura por zonas.
* **Iluminación:** Ajuste de intensidad y color de bombillas inteligentes.
* **Seguridad:** Estado de cerraduras y cámaras en tiempo real.
* **Energía:** Gráficos de consumo diario.

---

## ✨ Características Detalladas

### 🌗 Modo Oscuro Inteligente (Auto-Adaptativo)
A diferencia de las implementaciones básicas, este proyecto utiliza una arquitectura de variables CSS segregadas. El sistema detecta la preferencia global del sistema operativo, pero está preparado para ser sobreescrito mediante una clase maestra.

### 📱 Diseño "Mobile-First"
La interfaz ha sido construida bajo la metodología *Mobile-First*, asegurando que la experiencia en un panel de pared (tablet) o un smartphone sea tan fluida como en un ordenador de escritorio.

### ⚡ Rendimiento Óptimo
* **Zero dependencias:** No usa Bootstrap, jQuery ni frameworks pesados.
* **Iconografía SVG:** Todos los iconos son vectores ligeros que no pixelan y cargan instantáneamente.
* **Animaciones no intrusivas:** Micro-interacciones en los botones para dar feedback táctil al usuario.

---

## 🛠️ Stack Tecnológico

| Tecnología | Uso Principal |
| :--- | :--- |
| **HTML5** | Estructura semántica (Header, Main, Section, Aside). |
| **CSS3 (Grid/Flex)** | Maquetación responsiva y alineación de dispositivos. |
| **Custom Properties** | Gestión de temas (Colores, espaciados, sombras). |
| **Google Fonts** | Tipografía 'Inter' para máxima legibilidad. |

---

## 🌓 Lógica del Sistema de Temas

El núcleo del modo oscuro reside en el uso estratégico de `:root`. Aquí un ejemplo de cómo se gestiona la paleta de colores:

```css
/* Esquema de colores base (Light) */
:root {
    --primary-bg: #F4F7FE;
    --card-bg: #FFFFFF;
    --text-main: #2B3674;
    --accent: #4318FF;
    --shadow: rgba(0, 0, 0, 0.05);
}

/* Adaptación automática a Dark Mode */
    :root {
        --primary-bg: #0B1437;
        --card-bg: #111C44;
        --text-main: #FFFFFF;
        --shadow: rgba(0, 0, 0, 0.5);
    }
}

###FIGMA: https://www.figma.com/site/un902PjWAHiBeNSraeI6lo/Domus-Connect?node-id=0-1&p=f&t=nQTGBQzCh7ddJWR1-0
