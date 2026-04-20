# RWS Chatbot — Rival Wood Solutions

Asistente de atención al cliente integrado en el sitio web de RWS, construido con n8n y un AI Agent conectado a un modelo de lenguaje. Responde preguntas sobre servicios, materiales y proyectos de carpintería a la medida en tiempo real.

---

## Descripción

El sistema recibe mensajes desde un widget de chat embebido en el sitio web, los procesa a través de un flujo automatizado en n8n y devuelve una respuesta generada por IA al cliente. El agente mantiene contexto de la conversación mediante memoria de sesión y está configurado exclusivamente para responder temas relacionados con RWS.

---

## Tecnologías

- n8n (automatización del flujo)
- OpenAI GPT-4o-mini (modelo de lenguaje)
- HTML / JavaScript (frontend del chatbot)
- Google Sheets (registro de leads)
- Webhook (comunicación entre frontend y n8n)

---

```

El flujo tiene 7 nodos. El ciclo completo desde que el cliente envía el mensaje hasta que recibe respuesta tarda menos de 3 segundos.

---

## Requisitos

- Instancia de n8n activa (cloud o self-hosted)
- API Key de OpenAI
- Sitio web con acceso para modificar el HTML
- Cuenta de Google para el nodo de Sheets (opcional)

---

## Instalación

1. Clonar el repositorio o descargar los archivos.
2. Importar el archivo `rws_workflow.json` en n8n desde el menú **Import from File**.
3. Configurar las credenciales de OpenAI en el nodo **OpenAI Chat Model**.
4. Activar el workflow y copiar la URL del webhook que genera n8n.
5. Abrir `RWS.WED` y reemplazar el valor de `WEBHOOK_URL` con la URL copiada.

```javascript
// index.html — línea a modificar
function getWebhookUrl() {
  return "https://tu-instancia.n8n.cloud/webhook/rws-chatbot";
}
```


## Estructura de archivos

```
/
├── index.html              # Sitio web de RWS con el widget de chat integrado
├── rws_workflow.json       # Flujo de n8n exportado
├── uso_de_ia.md            # Registro del uso de IA durante el desarrollo
└── README.md
```

---


## Proyecto académico

Curso: Inteligencia Artificial Aplicada 
Empresa base: RWS - Rival Wood Solutions  
