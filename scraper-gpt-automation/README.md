# 🤖 Automatización GPT SCAPER / CAPTACIÓN DE LEADS EN AUTOMÁTICO - Buscar y contactar empresas automáticamente

Esta automatización está dividida en **2 automatizaciones conectadas** entre sí mediante Google Sheets.

---

## 🧩 AUTOMATIZACIÓN 1 (Parte 1) - Búsqueda de empresas a partir de un GPT personalizado creado por mí

1. Se lanza un **Webhook** en Make.com.
2. Se conecta a un **GPT personalizado** (llamado SCRAPER INFO NICHOS) que realiza una búsqueda de empresas de un nicho específico en una ciudad/país que tu le pidas.
3. Extrae la información y devuelve:
   - Nombre de la empresa
   - Correo electrónico de la empresa
   - Dirección de la empresa
   - Sitio Web de la empresa
4. Guarda los resultados en un Google Sheets llamado `GPT SCAPER INFO`.

### 🖼️ Vista del flujo:

![Flujo Parte 1](../assets/scraper-gpt-automation/PARTE%201%20-%20GPT%20SCAPER.png)

### 🧠 Instrucciones del GPT:

![Instrucciones GPT](../assets/scraper-gpt-automation/CONFIGURACI%C3%93N%20GPT%20SCAPER.png)

### 🔗 Enlace del GPT personalizado: https://chatgpt.com/g/g-67a0f1a2f3048191a9a64652e8bbf557-scraper-info-nichos

---

## ✉️ AUTOMATIZACIÓN 2 (Parte 2) - Envío de correos automatizados a las empresas que nos interesen

1. Cuando el usuario selecciona **"Sí"** en la columna **F** del Sheets...
2. Se activa un flujo Make.com:
   - Crea asunto y cuerpo con GPT.
   - Envía el email a la empresa correspondiente de esa fila del Google Sheets.
   - Actualiza la columna **E** con el estado de "Sin Enviar" a "Enviado".

### 🖼️ Vista del flujo:

![Flujo Parte 2](../assets/scraper-gpt-automation/PARTE%202%20-%20GPT%20SCAPER.png)

### 📊 Ejemplo de hoja de cálculo:

![Ejemplo de Google Sheets](../assets/scraper-gpt-automation/GOOGLE%20SHEETS%20-%20GPT%20SCAPER%20INFO.png)

---

## 📁 Archivos

- Carpeta `/assets/scraper-gpt/`: contiene capturas y visuales para esta automatización.
- Carpeta `/scraper-gpt-automation/`: contiene este `README.md`.

---

## ✍️ Autor

**Sergi Buendía**  
[github.com/sergibuendia](https://github.com/sergibuendia)
