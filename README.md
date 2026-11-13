# 📚 Library · Mayra Bastidas

Guías, ideas y reflexiones sobre tecnología, trabajo, cambio y lo que vaya surgiendo.

🌐 **Versión web (recomendada):** https://mayramb.github.io/library/

## Guías

| # | Guía | Para qué sirve |
|---|---|---|
| 01 | [Búsqueda de empleo en piloto automático](./busqueda-empleo-ia/) | Claude busca ofertas a diario, filtra, adapta tu CV y lo registra en Excel |
| 02 | [Difusión de la innovación](https://mayramb.github.io/diffusion_innovation_theory/) | Cómo se propaga el cambio en una organización |

## Cómo está organizada

```
library/
├── index.html          ← portada web (lee catalogo.json)
├── catalogo.json       ← lista de guías (aquí se añade cada guía nueva)
├── assets/style.css    ← diseño común
├── _plantilla/         ← copiar para crear una guía nueva
└── busqueda-empleo-ia/
    ├── index.html      ← visor (copia de _plantilla, no se edita)
    ├── README.md       ← la guía
    └── prompt-plantilla.md
```

## Añadir una guía nueva (3 pasos)

1. Copia la carpeta `_plantilla/` y renómbrala (ej. `excel-con-ia/`).
2. Escribe la guía en `README.md` dentro de esa carpeta.
3. Añade una entrada en `catalogo.json`.

---

¿Hablamos de esto? [Escríbeme](mailto:mayra.bastidas@synthesis-data.com) · [Synthesis Data](https://synthesis-data.com)
