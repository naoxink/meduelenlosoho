# meduelenlosoho
Extensión para Chrome que permite inyectar css y js en los sitios web

# Añadir CSS y JS personalizados a un sitio concreto
Para añadir CSS y/o JS a un sitio web sólo tendremos que crear su/s correspondiente/s `.js` y/o `.css` en la raíz de la carpeta (donde está el `manifest.json`). Después tendremos que añadir estos al `manifest.json` en la clave `content_scripts`:

```json
  "content_scripts": [
    {
      "matches": [  ], // URLs que coincidan
      "css": ["all.css"], // CSS (opcional)
      "js": ["all.js"] // JS (opcional)
    }
  ]
```

Después de cada modificación hay que recargar la extensión en Chrome. **No es necesario quitarla y volverla a añadir**, sólo recargarla.

# Instalar extensión descomprimida (desarrolladores)
https://developer.chrome.com/docs/extensions/mv3/getstarted/#unpacked
