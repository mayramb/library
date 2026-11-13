# 🔎 Tu búsqueda de empleo en piloto automático con IA

**Guía práctica para que Claude busque ofertas por ti todos los días, las filtre con tus criterios, te ajuste el CV y lo registre todo en un Excel.**

> Tú no aplicas a nada a ciegas. La IA investiga y prepara; **tú decides**.

---

## ¿Qué consigues?

Cada mañana, sin abrir nada, tienes:

1. ✅ Una lista corta de ofertas que **sí encajan** contigo (no 200 links basura).
2. ✅ El porqué de cada una (salario, seniority, empresa).
3. ✅ Tu CV **ya adaptado** a cada oferta.
4. ✅ Una fila nueva en tu Excel de seguimiento con fecha y link.

⏱️ Configuración: **1–2 horas una sola vez**. Después: 10 minutos al día para revisar.

---

## Lo que necesitas

| Pieza | Para qué | ¿Obligatorio? |
|---|---|---|
| Cuenta de Claude (plan de pago) | Ejecutar tareas programadas | Sí |
| App de escritorio de Claude | Que la tarea pueda leer/escribir en una carpeta de tu ordenador | Recomendado |
| Conector de **Indeed** | Búsqueda principal de ofertas | Recomendado |
| Conector de **Google Drive** (opcional) | Guardar CVs y Excel en la nube | No |
| Tu **CV maestro** (.docx) | La fuente de la que salen todos los CVs adaptados | Sí |
| Un **Excel de seguimiento** | Registrar cada oferta | Sí (plantilla abajo) |

---

## Paso a paso

### Paso 1 · Prepara tu CV maestro
Un solo documento con **todo**: todos los puestos, fechas, logros con métricas, educación y certificaciones. Es largo a propósito: la IA **recorta** según cada oferta, pero nunca inventa.

> 💡 Regla de oro: la IA solo puede usar lo que está en tu maestro. Si un logro no está ahí, no aparecerá en ningún CV.

### Paso 2 · Crea tu carpeta de trabajo
```
📁 Busqueda-Empleo/
   ├── CV_MAESTRO.docx
   ├── Seguimiento_Ofertas.xlsx
   └── 📁 CVs_ajustados/
```

### Paso 3 · Crea el Excel de seguimiento
Columnas mínimas (fila 1 = encabezados):

| A | B | C | D | E | F | G | H | I |
|---|---|---|---|---|---|---|---|---|
| ID (`=C2&D2`) | Fecha | Empresa | Puesto | Link | Por qué califica | Salario | CV ajustado | ¿Aplicado? |

- La columna **A** evita duplicados (empresa + puesto).
- La columna **I** la rellenas **tú** a mano.

### Paso 4 · Define tus criterios (lo más importante)
Antes de escribir el prompt, responde en un papel:

1. **Puestos**: 3–5 títulos que buscas (ej. "PMO", "Data Governance Manager").
2. **Ubicación**: ciudad y/o remoto.
3. **Salario mínimo** aceptable.
4. **Seniority**: qué niveles sí y cuáles no (ej. nada junior).
5. **Tipo de empresa / contrato**: multinacional, indefinido, sector…
6. **Descartes automáticos**: lo que nunca quieres ver.

> Si tus criterios son vagos, la IA te traerá basura. Esta parte **no** se la delegues.

### Paso 5 · Escribe el prompt
Copia la plantilla de [`prompt-plantilla.md`](./prompt-plantilla.md) y sustituye todo lo que va entre `[CORCHETES]`.

### Paso 6 · Prueba manual primero
Pega el prompt en un chat normal de Claude y ejecútalo **una vez**. Revisa:
- ¿Las ofertas encajan de verdad?
- ¿Los links funcionan?
- ¿El CV adaptado respeta tus fechas y cargos?

Ajusta el prompt y repite hasta que te guste el resultado. **No programes algo que no has probado.**

### Paso 7 · Prográmalo
En Claude, crea una **tarea programada** con el prompt final:
- **Frecuencia**: diaria (laborables) o semanal.
- **Hora**: temprano, para tenerlo al empezar el día.
- **Carpeta**: dale acceso a tu carpeta `Busqueda-Empleo`.
- **Aprobaciones**: la primera semana, deja que te pida permiso; cuando confíes, actívala en automático.

### Paso 8 · Rutina diaria (10 min)
1. Abre el resumen del día.
2. Lee el "por qué califica" de cada oferta.
3. Revisa el CV adaptado → aplica tú.
4. Marca la columna **I** del Excel.

---

## Errores típicos (y cómo evitarlos)

| Problema | Solución |
|---|---|
| Trae ofertas que no encajan | Criterios más estrictos en el Paso 4 |
| El link es de la web de búsqueda, no de la oferta | Exige en el prompt "link directo a la oferta" |
| El CV inventa o resume de más | Añade: "no inventes nada; conserva todos los puestos y fechas" |
| El CV dice "sin experiencia en X" | Añade: "nunca menciones lo que no tengo; simplemente omítelo" |
| Se repiten ofertas | Pide comprobar la columna A antes de añadir filas |
| Un día no hay nada bueno | Pide que lo diga explícitamente en vez de forzar resultados |

---

## Reglas de seguridad (no negociables)

- 🚫 La IA **no aplica** a ofertas ni **contacta** a reclutadores. Eso lo haces tú.
- 🔒 No metas en el prompt datos sensibles (DNI, situación migratoria, cuentas bancarias).
- 👀 Revisa siempre el CV antes de enviarlo. La IA prepara; tú firmas.

---

## Siguientes mejoras (cuando lo básico funcione)

- Añadir más fuentes (LinkedIn, portales de tu sector, bolsa de tu escuela).
- Una pestaña **Dashboard** en el Excel: tasa de respuesta, entrevistas, ofertas por semana.
- Una segunda tarea semanal que te prepare preguntas de entrevista para las ofertas que aplicaste.

---

<div data-solo-github>

### ¿Prefieres que te lo deje funcionando?
Lo configuramos juntos en una sesión de 90 minutos, adaptado a ti o a tu negocio.
👉 [Escríbeme](mailto:mayra.bastidas@synthesis-data.com?subject=Quiero%20montarlo%20contigo) · [Synthesis Data](https://synthesis-data.com) · [Más guías en la Library](https://mayramb.github.io/library/)

</div>

*Guía creada por **Mayra Bastidas**. Si te sirve, compártela.*
