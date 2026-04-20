# Uso de IA en el Desarrollo del Proyecto — RWS Chatbot

Durante el desarrollo del proyecto se utilizaron distintas herramientas de IA como apoyo personal para resolver dudas técnicas, escribir código y tomar decisiones de diseño.

---

## Herramientas utilizadas

| Herramienta  | Para qué se usó |
|--------------|-|
| **ChatGPT**  | Diseño del flujo en n8n, configuración de nodos y resolución de errores |
| **Claude**   | Guia para utilizar GoogleSheets y crear el api
| **DeepSeek** | Consultas técnicas de JavaScript y validación de lógica |
| **Cursor**   | Edición del HTML del sitio web con sugerencias de código en tiempo real |

---

## Prompts destacados

### Diseño del flujo


```
"Quiero que el chatbot se presente primero, y que solo funcione para el tema de
ventas de muebles. Si pregunta cualquier otra cosa que responda de manera cortés
que no está creado para eso."
```

---

### Configuración del agente

```
"¿Qué expresión uso en n8n para leer el campo message del body del POST?"
```

```
"Dame el system message correcto para el agente de RWS que solo responda temas
de muebles y se presente automáticamente."
```

```
"¿Por qué el nodo Respond to Webhook me devuelve vacío si el agente sí genera respuesta?"
```
---

### Lógica y casos borde

```
"¿Qué información guarda en Google Sheets si el cliente solo dice su nombre
y no se sabe si es mayorista o minorista?"
```
```
"¿Cómo restrinjo el agente para que no responda temas fuera de muebles aunque el cliente insista?"
```

---


## Conclusión

El uso de IA permitió avanzar más rápido en las partes técnicas del proyecto, especialmente en la configuración de n8n y la integración con el frontend. No reemplazó el trabajo propio, sino que sirvió de guía para tomar mejores decisiones técnicas durante el desarrollo.

---

*Proyecto: RWS - Rival Wood Solutions | Curso: IA y Automatización | 2025*
