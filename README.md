# Banco de fotos

Archivo de imágenes etiquetadas. Cada foto vive en `fotos/` y su ficha en `catalogo.json`.

Si buscas una frase y esa frase está en `phrases` (o coincide con el título, la descripción o las etiquetas), aparece la imagen.

## Cómo está etiquetada una foto

```json
{
  "id": "playa",
  "file": "playa.jpg",
  "title": "Orilla en calma",
  "caption": "La marea baja deja el sol tendido sobre la arena mojada.",
  "phrases": ["atardecer en la playa", "puesta de sol en el mar"],
  "tags": ["playa", "atardecer", "mar", "arena"],
  "place": "Costa",
  "year": 2024
}
```

`phrases` son las frases que deben encontrar esa foto. Los acentos no importan: `cafe de la manana` encuentra `café de la mañana`.

## Añadir una foto al archivo

1. Guarda el jpg en `fotos/nombre.jpg`.
2. Suma un objeto al arreglo de `catalogo.json`, con al menos una frase.
3. Al publicar, la búsqueda de esa frase muestra la imagen.

La página también deja guardar fotos solo en el navegador. Esas no entran al repositorio.
