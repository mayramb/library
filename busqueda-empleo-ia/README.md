# 🔎 Tu búsqueda de empleo en piloto automático con IA

**Cada madrugada, Claude busca ofertas, descarta las que no encajan, te prepara un CV adaptado a cada una y lo registra todo en un Excel.**

> La IA investiga y prepara. **Tú decides y postulas.** Nunca aplica ni contacta a nadie.

---

## Qué recibes cada mañana

1. ✅ Una tabla corta con las ofertas que **sí** encajan y por qué.
2. ✅ Un **CV en Word adaptado** a cada una, partiendo de tu CV maestro.
3. ✅ Filas nuevas en tu **Excel de seguimiento**.
4. ✅ La lista de lo descartado y el motivo.

⏱️ Montarlo: 2–3 horas una vez. Después: 10 minutos al día.

---

## Las piezas

| Pieza | Para qué |
|---|---|
| **Claude (app de escritorio)** con una carpeta conectada | Lee tus archivos y escribe CVs y Excel |
| **Tarea programada** diaria | Ejecuta el prompt sola, de madrugada |
| **Conector de empleo** (Indeed) + búsqueda web | Fuentes de ofertas |
| **CV maestro ATS** (uno por idioma) | La base de todos los CVs. Nunca se crea desde cero |
| **Archivo de HECHOS** (.md) | Tus logros y cifras reales. Evita que la IA invente |
| **Excel de seguimiento** | Registro para medir qué funciona |

---

## Paso a paso

### Paso 1 · Prepara tu carpeta
```
📁 Busqueda-Empleo/
   ├── CV_[Nombre]_ATS_Espanol.docx
   ├── CV_[Nombre]_ATS_English.docx
   ├── HECHOS_[Nombre]_para_CVs.md
   └── Seguimiento_Ofertas.xlsx
```
- **CV maestro ATS:** texto plano, sin tablas ni columnas ni iconos, contacto en el cuerpo (no en el encabezado).
- **Archivo de HECHOS:** tus experiencias con cifras verificadas, herramientas que sí dominas, certificaciones que sí tienes y una sección **"Datos prohibidos"** con lo que la IA no debe afirmar nunca.

> 💡 El archivo de HECHOS es la pieza que más calidad aporta. Cuanto más concreto, menos inventa la IA.

### Paso 2 · Arma el Excel de seguimiento
Crea una **tabla de Excel con nombre** (Insertar → Tabla, nómbrala `Tabla1`) con estas columnas:

| Col | Contenido | Quién |
|---|---|---|
| A | ID: fórmula `=D2&E2` (detecta ofertas repetidas) | Fórmula |
| B | Fecha de la búsqueda (fecha real, no texto) | IA |
| C | Vía: **A** = salario ideal · **B** = puente realista | IA |
| D | Empresa | IA |
| E | Título | IA |
| F | Link directo a la oferta | IA |
| G | Carril + por qué calificó | IA |
| H | Salario o "No visible" | IA |
| I | Nombre del CV generado | IA |
| J | Aplicado (SI / NO) | Tú |
| K | Razón para no aplicar | Tú |
| L | Respuesta | Tú |
| M | Fecha de respuesta | Tú |
| N | Status | Tú |
| O | Días hasta respuesta: `=SI(M2="";"";M2-B2)` | Fórmula |

Separar lo que rellena la IA de lo que rellenas tú es lo que luego te permite **medir qué funciona**.

> 📥 ¿Prefieres mi plantilla ya hecha, con estadísticas y gráfico? [Pídemela por correo](mailto:mayra.bastidas@synthesis-data.com?subject=Plantilla%20Excel%20-%20B%C3%BAsqueda%20de%20empleo%20con%20IA).

### Paso 3 · Escribe tu prompt (lo más importante)
👉 **Copia la plantilla: [prompt-plantilla.md](./prompt-plantilla.md)** y sustituye todo lo que va entre `[CORCHETES]`.

Antes, define en un papel:
- **Carriles:** 2 perfiles distintos que buscas, con títulos concretos (ej. "Data Governance Manager", no "Manager").
- **Vías salariales:** A = tu objetivo ideal · B = el mínimo aceptable como puente.
- **Exclusiones:** empresas, sectores y tipos de rol que no quieres nunca.
- **Señales de descarte:** palabras que delatan junior, rol técnico, venta pura, etc.

### Paso 4 · Pruébalo a mano
Pega el prompt en un chat normal de Claude con la carpeta conectada y ejecútalo **una vez**. Revisa que las ofertas encajan, que los links funcionan y que el CV no inventa nada. Ajusta y repite.

### Paso 5 · Prográmalo
Pídele a Claude: *"Crea una tarea programada diaria a las 4:00 con este prompt"*. Puedes pausarla o editarla cuando quieras.

> ⚠️ Deja el Excel **cerrado** por la noche. Si está abierto, la IA no puede escribir en él.

---

## Lecciones aprendidas (4 meses de uso)

| Problema | Solución (ya incluida en el prompt) |
|---|---|
| La IA inventaba logros o herramientas | Archivo de HECHOS + datos prohibidos + verificación final |
| CVs desde cero perdían el formato ATS | "Parte SIEMPRE del maestro" |
| Se colaban ofertas caducadas | Descartar lo publicado hace más de 45 días |
| Agregadores cambiaban títulos o modalidad | Verificar en la web de la empresa o LinkedIn |
| Escribía la fecha de publicación, no la de búsqueda | Regla explícita de fecha |
| Escribía en filas vacías equivocadas del Excel | Buscar la última fila por la columna Empresa |
| Decía que guardó el Excel sin hacerlo | Reabrir, contar filas y, si falla, guardar un CSV |
| Términos amplios llenaban el informe de ruido | Solo títulos con calificador |

### 📊 La lección más valiosa: mide y reasigna
Al mes revisé el Excel: un carril tenía **50 % de respuesta** y el otro **26 %**, pero la tarea traía 3 veces más ofertas del peor. El problema era de configuración, no de mercado. Cambié el prompt para dedicar ~65 % de la búsqueda al carril que funcionaba.

**El Excel no es burocracia: es lo que te permite mejorar el sistema con datos.**

---

## Reglas no negociables
- 🚫 La IA no aplica ni contacta a reclutadores.
- 🔒 Tus datos de contacto van fijos en el CV maestro; la IA nunca los genera.
- 👀 Revisa cada CV antes de enviarlo.
- 📉 Si un día no hay nada bueno, el informe lo dice. No se baja el listón.

---

## 📥 ¿Quieres mi plantilla de Excel o más detalle?
Te envío la plantilla lista para usar (con las fórmulas, estadísticas por día y gráfico) o lo vemos juntos.

👉 **[Pídeme la plantilla](mailto:mayra.bastidas@synthesis-data.com?subject=Plantilla%20Excel%20-%20B%C3%BAsqueda%20de%20empleo%20con%20IA)** · [Synthesis Data](https://synthesis-data.com) · [Más en la Library](https://mayramb.github.io/library/)

---

*Guía creada por **Mayra Bastidas**. Si te sirve, compártela.*
