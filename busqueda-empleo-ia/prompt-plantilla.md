# Plantilla de prompt · Búsqueda de empleo diaria

Copia todo el bloque de abajo y sustituye lo que está entre `[CORCHETES]`.

```
Eres mi asistente de búsqueda de empleo. Ejecuta esta tarea de investigación.
NO apliques a ninguna oferta ni contactes a nadie: solo investiga, filtra,
adapta mi CV y registra los resultados.

== MI PERFIL ==
Busco empleo en [CIUDAD / PAÍS] (o remoto [PAÍS]) en roles de [ÁREA PRINCIPAL].
Sectores preferidos: [SECTOR 1], [SECTOR 2] (no descartes otros si el resto encaja).
Salario objetivo: [X–Y €/año brutos].

== QUÉ BUSCAR ==
Términos de búsqueda:
- "[PUESTO 1]"
- "[PUESTO 2]"
- "[PUESTO 3]"

== FUENTES ==
1. Conector de Indeed (país "[CÓDIGO PAÍS]", ubicación "[CIUDAD]" y una pasada con "remote").
2. Búsqueda web en lenguaje natural (sin operadores site: ni booleanos) para cubrir
   LinkedIn y otros portales. Ej.: "[PUESTO 1] [CIUDAD] empleo".
3. Para ofertas prometedoras, abre el link individual y saca el detalle
   (salario, seniority, requisitos) antes de decidir.
4. Si la oferta está cerrada o "ya cubierta", descártala.

== FILTRO (evalúa cada oferta) ==
1. ¿Salario visible o inferible ≥ [MÍNIMO]? (si no es visible, marca "no visible";
   no descalifica por sí solo)
2. ¿Seniority real (en el cuerpo de la oferta, no solo el título) es
   [NIVELES ACEPTADOS]? Descarta junior/prácticas.
3. ¿Tipo de empresa/contrato: [CRITERIO, ej. multinacional, indefinido]?
4. [CRITERIO PROPIO ADICIONAL]
Incluye solo las que cumplan al menos [N] de [4] criterios.

== CV ADAPTADO (por cada oferta que califique) ==
- Parte SIEMPRE de mi CV maestro: [RUTA/NOMBRE DEL CV MAESTRO].
- Conserva todos los puestos y fechas. No inventes nada.
- Elige qué logros destacar según la oferta y quita lo irrelevante.
- Formato ATS limpio: texto plano, sin tablas ni gráficos.
- Idioma del CV = idioma de la oferta.
- Nunca menciones lo que no tengo ("sin experiencia en X"): simplemente omítelo.
- Guarda como: [CARPETA]/CVs_ajustados/CV_[Empresa]_[Puesto]_[AAAA-MM-DD].docx

== REGISTRO EN EXCEL ==
Archivo: [CARPETA]/Seguimiento_Ofertas.xlsx, hoja "[NOMBRE HOJA]".
- Antes de añadir, comprueba que Empresa+Puesto no exista ya (columna A).
- Añade una fila por oferta nueva en las columnas B a H:
  B Fecha de hoy · C Empresa · D Puesto · E Link DIRECTO a la oferta
  (si no hay link directo, escribe "link directo no disponible" + la fuente)
  · F Por qué califica (1 línea) · G Salario · H Nombre del CV ajustado
- Copia la fórmula de la columna A en la nueva fila.
- No toques la columna I ni el formato existente.

== ENTREGA EN EL CHAT ==
1. Una línea: cuántas ofertas revisaste vs. cuántas calificaron, y si alguna
   fuente falló.
2. Tabla: Empresa | Puesto | Link | Por qué califica | Salario | CV.
3. Si ninguna califica, dilo claramente. No fuerces resultados débiles.
```

---

### Consejos para ajustarlo
- Empieza con **3 términos de búsqueda**, no 10. Amplía después.
- Si recibes demasiadas ofertas, sube el número de criterios exigidos en el filtro.
- Si recibes muy pocas, añade "remoto" o un sector más.
