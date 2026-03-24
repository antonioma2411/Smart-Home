# 🏠 SmartHome Dashboard: Control Residencial Inteligente


**SmartHome Dashboard** es una plataforma web estática de alto rendimiento diseñada para centralizar el control de dispositivos IoT (Internet of Things). El proyecto demuestra el uso de técnicas avanzadas de CSS moderno, como el manejo de estados visuales, diseño de tarjetas interactivas y una transición fluida entre modos de iluminación.

A diferencia de las implementaciones basadas únicamente en las preferencias del sistema, este proyecto incluye un **conmutador de tema manual (botón)**. Esto permite al usuario sobrescribir el modo de luz o la oscuridad en cualquier momento, ofreciendo una experiencia de usuario superior.

---

## 🚀 Vista Rápida

El objetivo de este proyecto es ofrecer una interfaz minimalista pero potente donde el usuario pueda monitorear:
* **Climatización:** Control de temperatura por zonas.
* **Iluminación:** Ajuste de intensidad y color de bombillas inteligentes.
* **Seguridad:** Estado de cerraduras y cámaras en tiempo real.
* **Energía:** Gráficos de consumo diario.

---

## ✨ Características Detalladas

### 🌗 Control de Tema Manual (Boton)
La interfaz incluye un botón dedicado que permite al usuario alternar instantáneamente entre el modo claro y el oscuro. El tema seleccionado se aplica globalmente y la transición es suave para evitar la fatiga visual.


### 📱 Diseño "Mobile-First"
La interfaz ha sido construida bajo la metodología *Mobile-First*, asegurando que la experiencia en un panel de pared (tablet) o un smartphone sea tan fluida como en un ordenador de escritorio.

### ⚡ Rendimiento Óptimo
* **Zero dependencias de frameworks:** No usa Bootstrap ni frameworks pesados.
* **Animaciones no intrusivas:** Micro-interacciones en los botones para dar feedback táctil al usuario.

---

## 🛠️ Stack Tecnológico

| Tecnología | Uso Principal |
| :--- | :--- |
| **HTML5** | Estructura semántica (Header, Main, Section). |
| **CSS3 (Grid/Flex)** | Maquetación responsiva y alineación de dispositivos. |
| **Custom Properties** | Gestión de temas y colores dinámicos. |
| **Google Fonts** | Tipografía 'Inter' para máxima legibilidad. |

---


###FIGMA: https://www.figma.com/site/un902PjWAHiBeNSraeI6lo/Domus-Connect?node-id=0-1&p=f&t=nQTGBQzCh7ddJWR1-0


## 🌓 Lógica del Sistema de Temas

El núcleo del sistema de temas reside en el uso estratégico de `:root` y clases de CSS. Cuando se activa el modo oscuro, JavaScript añade una clase (ej. `.dark-mode`) al cuerpo de la página, lo que sobrescribe las variables de color predeterminadas.

Aquí un ejemplo de cómo se gestiona la paleta de colores:

```css
/* Esquema de colores predeterminado (Claro) */
:root {
    --primary-bg: #F4F7FE;
    --card-bg: #FFFFFF;
    --text-main: #2B3674;
    --accent: #4318FF;
    --shadow: rgba(0, 0, 0, 0.05);
}

/* Esquema de colores para el Modo Oscuro */
:root.dark-mode {
    --primary-bg: #0B1437;
    --card-bg: #111C44;
    --text-main: #FFFFFF;
    --shadow: rgba(0, 0, 0, 0.5);
}

