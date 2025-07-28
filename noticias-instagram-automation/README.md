# 📰 Automatización para publicar noticias de IA en Instagram (LogicApps + Make)

Automatización desarrollada para un proyecto del máster en Inteligencia Artificial & Machine Learning for Business, dentro de la asignatura de *Tecnologías Cloud: Frameworks y proyectos de IA*. El objetivo es extraer noticias relacionadas con la IA y publicarlas automáticamente en Instagram.

---

## ⚙️ ¿Cómo funciona?

### 📌 Parte 1 - Automatización en Logic Apps (Azure)

- Se ejecuta con un trigger de tipo `Recurrence` (frecuencia personalizada).
- Se conecta a la **API de NewsAPI.org** para obtener noticias sobre *Tecnología* e *Inteligencia Artificial*.
- Se usa `Parse JSON` y `Initialize Variables` para estructurar la información.
- A través de la **API de ChatGPT**, se reescribe el contenido como si fuera un *post profesional de Instagram*.
- Finalmente, se envía la información procesada a **Make.com** mediante un Webhook.

### 🤖 Parte 2 - Automatización en Make.com

- Se activa con el Webhook anterior.
- Utiliza **DALL·E 3** para generar una imagen relacionada con la noticia.
- Publica automáticamente en **Instagram**, usando como caption la noticia resumida y la imagen generada.

---

## 💡 Notas

> Esta automatización también se podría realizar 100% en Make.com, pero gracias a esta asignatura del máster he podido aprender a trabajar con Logic Apps y complementar herramientas low-code.

---

## 📸 Capturas de pantalla

(Próximamente se añadirán imágenes ilustrativas aquí)

---

## 🔗 Autor

**Sergi Buendía**  
[GitHub](https://github.com/sergibuendia)
