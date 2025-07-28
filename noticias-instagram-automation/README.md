# 📰 Automatización para publicar noticias de IA en Instagram (LogicApps + Make)

Automatización desarrollada para un proyecto del máster en Inteligencia Artificial & Machine Learning for Business (EAE Business School, Barcelona), dentro de la asignatura de *Tecnologías Cloud: Frameworks y proyectos de IA*. El objetivo es extraer noticias relacionadas con la IA y con la tecnología, y publicarlas automáticamente en Instagram.

---

## ⚙️ Descripción del Proyecto

Esta automatización se divide en dos partes:

---

### 📌 **Parte 1 - Extracción y preparación del contenido con Logic Apps (Microsoft Azure)**

En esta parte se realiza lo siguiente:

1. Se utiliza un **trigger de tipo "Recurrence"** para ejecutar la automatización de forma periódica.
2. Conectamos a la **API de NewsAPI.org** para obtener noticias relacionadas con **Tecnología e Inteligencia Artificial**.
3. Se pasan por módulos intermedios como:
   - `Parse JSON`: para interpretar correctamente los datos de la API.
   - `Initialize variables`: útil para almacenar temporalmente información estructurada.
4. A través de la **API de ChatGPT (OpenAI)** se reescribe la noticia para adaptarla como pie de foto para Instagram.
5. Finalmente, se realiza una **llamada a un webhook de Make.com** para pasar la información a la segunda parte.

**📷 Capturas de pantalla relevantes de la primera parte de la automatización:**
- ![PARTE 1 - Automatización Logic APPS](../assets/noticias-instagram-automation/PARTE%201%20-%20Automatización%20Logic%20APPS.png)
- ![PROMPT API ChatGPT (LogicApps)](../assets/noticias-instagram-automation/PROMPT%20API%20ChatGPT%20(LogicApps).png)

### 🤖 **Parte 2 - Generación de imagen y publicación automática en **Instagram con Make.com**
Una vez recibido el contenido desde Logic Apps, esta segunda automatización realiza:

1. **Recepción del webhook** con los datos de la noticia ya formateada y resumida.
2. Se genera una imagen con **DALL·E 3 (vía módulo de OpenAI)** en base a la noticia recibida.
3. Se utiliza el módulo de **Instagram for Business** para publicar automáticamente:
   - En el campo *caption* se coloca el texto generado.
   - Se sube la imagen generada automáticamente por DALL·E.

**📷 Capturas de pantalla relevantes de la segunda parte de la automatización:**
- ![PARTE 2 - Automatización Make.com (Publicar noticia en Instagram)](../assets/noticias-instagram-automation/PARTE%202%20-%20Automatización%20Make.com%20(Publicar%20noticia%20en%20Instagram).png)
- ![PROMPT DALL-E (Generación de imagen para publicación en Instagram)](../assets/noticias-instagram-automation/PROMPT%20DALL-E%20(Generación%20de%20imagen%20para%20publicación%20en%20Instagram).png)

---

## 💡 Notas

> Es importante destacar que esta automatización también se podría realizar 100% en Make.com, pero gracias a esta asignatura del máster he podido aprender a trabajar con Logic Apps y complementar herramientas low-code.

---

## 📁 Archivos del Proyecto

- `/noticias-logicapps.json` → Automatización de Logic Apps exportada en formato JSON.
- `/README.md` → Documentación de esta automatización.
- `/assets/noticias-instagram-automation/` → Carpeta con todas las capturas del flujo.

---

## 🔗 Autor

**Sergi Buendía**  
[GitHub](https://github.com/sergibuendia)
