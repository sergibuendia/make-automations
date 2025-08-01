# 🤖 Community Manager Automatizado (Creación y Publicación de Contenido en RRSS en automático)

Esta automatización combina dos automatizaciones conectadas entre sí para generar y publicar contenido en redes sociales (Instagram, LinkedIn y Facebook) de manera completamente automática a partir de ideas listadas en un Google Sheets.

---

## ⚙️ ¿Como funcionan las automatizaciones?

### 🧩 Automatización 1 (Parte 1) – Creación de contenido

A partir de un Google Sheets con ideas y descripciones de dicha idea, se genera:

- ✍️ El contenido textual de los posts para cada red social.
- 🧠 Generación automática de la imagen del post con un módulo de DALL·E (para Instagram).
- 🗂 Registro del contenido de los posts en un nuevo Google Sheets (rol de Community Manager), con una columna en la cual aprobaremos o no dicho contenido para publicar.

📍 Esta automatización se activa automáticamente cada vez que se añade una nueva idea al Google Sheets.

#### 🖼️ Vista del escenario Make.com

![Automatización creación de contenido](../assets/community-manager-automation/PARTE%201%20-%20Automatizaci%C3%B3n%20creaci%C3%B3n%20contenido%20RRSS.png)

#### 🗂️ Sheets con ideas y descripciones

![Google Sheets Ideas](../assets/community-manager-automation/GOOGLE%20SHEETS%20-%20Ideas%20y%20descripciones.png)

#### 🗂️ Sheets del Community Manager (pendiente/aprobado)

![Google Sheets CM](../assets/community-manager-automation/GOOGLE%20SHEETS%20-%20Community%20Manager.png)

---

### 🚀 Automatización Parte 2 – Publicación automática

Cuando el contenido es marcado como `Aprobado`, esta segunda automatización se activa y:

- 🗓 Publica automáticamente el contenido en Instagram, LinkedIn y Facebook.
- 🔁 Actualiza el estado de la publicación en el Google Sheets a `Publicado`.
- 🧠 En caso necesario, genera una nueva imagen con DALL·E (si se desea reemplazar la anterior).

#### 🖼️ Vista del escenario Make.com

![Automatización publicación de contenido](../assets/community-manager-automation/PARTE%202%20-%20Automatizaci%C3%B3n%20publicaci%C3%B3n%20RRSS.png)

#### 📱 Capturas de publicaciones reales

![Instagram Feed](../assets/community-manager-automation/POSTS%20GENERADOS%20EN%20INSTAGRAM.png)

---

## 🧩 Archivos JSON

Este repositorio contiene:

- `community-manager-create-content.json`: Automatización Parte 1
- `community-manager-post-content.json`: Automatización Parte 2

Puedes importar estos archivos directamente en Make.com para tener las automatizaciones listas para editar o ejecutar.

---

## 🧠 Conclusión

Gracias a la integración de herramientas como **Google Sheets**, **OpenAI (ChatGPT + DALL·E)** y **Make.com**, este sistema permite gestionar contenido de redes sociales de principio a fin sin intervención manual, reduciendo tiempos y facilitando la coherencia del mensaje en múltiples canales.

