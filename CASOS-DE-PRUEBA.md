# Casos de prueba manuales

Estos escenarios son regresiones mínimas para comprobar que las reglas de perfil y el informe se mantienen coherentes después de cambiar el cuestionario o la puntuación.

| Caso | Respuestas relevantes | Resultado esperado |
|---|---|---|
| Marca consolidada | Todas A; Q9 = A | Marca consolidada, puntuación 100/100 y tres recomendaciones de optimización. |
| Marca desalineada | Q3 = D; resto A | Marca desalineada; el índice global se limita por la debilidad crítica. |
| Marca en construcción | Q1 = D y Q2 = D; resto A | Marca en construcción; no se oculta la falta de fundamentos con una media alta. |
| Marca dispersa | Q5 = D y Q6 = D; resto A | Marca dispersa; coherencia es la dimensión crítica. |
| Marca funcional | Q7 = C y Q8 = C; resto A | Marca funcional; diferenciación y personalidad son la principal debilidad. |
| Caso mixto con empate | Todas B; Q9 = B | Marca dispersa como desempate secundario declarado; no se usa construcción por defecto. |
| Diferenciación débil | Q7 = D y Q8 = A; resto A | Marca funcional; índice ajustado máximo de 74 por una dimensión por debajo de 60. |

## Verificaciones funcionales

## Formato del informe y PDF

- [x] El informe web usa la paleta EA y jerarquía tipográfica ampliada.
- [x] El resultado incluye un gráfico radial SVG con cinco ejes, cinco marcadores con iconos de marca y una leyenda numérica.
- [x] Las tarjetas y recomendaciones conservan contraste adecuado en escritorio y móvil.
- [x] La portada PDF incorpora marca gráfica y una «X» dorada de baja opacidad.
- [x] Las cinco páginas A4 tienen iconos de marca en los encabezados interiores y colores consistentes para la puntuación.
- [x] Prueba automatizada: diagnóstico completo, tres recomendaciones, PDF descargable de cinco páginas, sin errores JavaScript.
- [x] Prueba móvil a 390 px: sin desbordamiento horizontal.
- [x] Verificación de límites de texto PDF: el contenido de las cinco páginas se mantiene dentro de la zona imprimible.


- [x] El código JavaScript pasa `node --check`.
- [x] Los cinco perfiles se activan en escenarios diseñados para ellos.
- [x] Cada escenario de resultado muestra tres recomendaciones.
- [x] La web pública genera un PDF de cinco páginas A4 con el gráfico radial de cinco dimensiones.
- [x] Navegación de escritorio y flujo completo en móvil verificados con navegador automatizado.
- [x] No se registraron errores JavaScript durante estas pruebas.
- [x] GitHub Pages está publicado y la URL pública se ha probado directamente.
- [ ] Revisar el diseño visual del PDF y validarlo con empresas reales antes del lanzamiento comercial.



## Simplificación de lectura del formulario (octubre 2026)

- [x] Se eliminan los 10 textos auxiliares situados bajo las preguntas; se conserva la descripción principal de cada sección.
- [x] La pregunta 9 sigue en la posición 9 de 10 y ofrece cuatro respuestas (A–D), igual que las demás.
- [x] En móvil, el aviso de privacidad queda a 28 px de la línea superior del pie de página.
- [x] La tarjeta «Tres próximos pasos» queda separada 20 px de la tarjeta del perfil.
- [x] Flujo completo: 10 preguntas, tres recomendaciones, PDF de cinco páginas A4, sin errores JavaScript ni desbordamiento horizontal a 390 px.

## Actualización del cuestionario y refinamiento editorial del PDF

- [x] La pregunta 9 mantiene la décima posición dentro del cuestionario, pero ofrece cuatro opciones, como las otras preguntas.
- [x] El criterio de desempate de perfiles solo usa opciones existentes de Q9 (A-D).
- [x] Portada PDF renovada con panel rosa pálido, tarjeta blanca para la puntuación y acentos corporativos.
- [x] Gráfico radial PDF calculado con las cinco puntuaciones reales, con polígono cerrado, relleno rosa, marcadores y cinco etiquetas dentro de los márgenes.
- [x] Página de acciones con badges numerados grandes, etiqueta «PASO» y título compactos, y bandas suaves para «Por qué importa».
- [x] Las listas de validación usan badges numerados alineados con su texto; el cierre oscuro incorpora acentos rosa y dorado.
- [x] Prueba de navegador con respuestas variadas: 4 opciones en cada una de las 10 preguntas, puntuaciones diversas, 3 recomendaciones y PDF A4 de 5 páginas.
- [x] Extracción de texto y límites: el contenido permanece dentro de la zona imprimible; el cuestionario no presenta desbordamiento horizontal en móvil.

## Revisión de paleta visual

- [x] Carbón `#29272A` sustituye al verde oscuro en los bloques y botones principales.
- [x] Fondo marfil `#F5F2ED` aplicado al fondo general y blanco cálido `#FFFEFC` a las tarjetas.
- [x] Rosa EA `#EA5A77` aplicado a acentos, progreso, selección y botón principal.
- [x] Verde EA `#46B382` aplicado a estados interactivos y al contorno del gráfico radial.
- [x] Dorado EA `#D2A158` aplicado a barras de dimensión y detalles gráficos.
- [x] Fondo marfil `#F5F2ED` y carbón `#29272A` conservados.
- [x] Los textos pequeños se mantienen en carbón o gris legible, no en dorado claro.
- [x] PDF adaptado a la misma paleta.
- [x] Los círculos decorativos se sustituyen por los iconos de la marca en cabecera, portada y listas del PDF.
- [x] Los puntos de datos del gráfico radial usan los símbolos de la marca.
- [x] El estado hover y foco de las opciones usa dorado, no verde.
- [x] El botón «Comenzar auditoría» mantiene buena visibilidad cuando está desactivado (borde rosa y texto claro) y cuando está activo (fondo rosa y texto carbón).
- [x] Navegador automatizado sobre la URL pública: comprobados los colores calculados y descarga de PDF de cinco páginas A4.


## Simplificación del informe: puntuaciones y fortalezas

- [x] Los porcentajes de las cinco dimensiones aparecen una sola vez en la tarjeta de dimensiones.
- [x] Se elimina la segunda leyenda con barras y puntuaciones del gráfico radial.
- [x] El lateral del gráfico radial muestra «Fortalezas y atención», «Qué destaca en tus respuestas», «Fortalezas declaradas» y «Áreas a revisar».
- [x] Se retira el panel duplicado de fortalezas de la parte inferior.
- [x] Se eliminan los iconos repetidos junto a las dimensiones, en las listas y en los vértices del gráfico.
- [x] El PDF sigue en cinco páginas A4; la página del gráfico coloca fortalezas y áreas de revisión junto al gráfico sin repetir las puntuaciones numéricas.
- [x] Pruebas de escritorio y móvil: cinco dimensiones, tres recomendaciones, sin desbordamiento horizontal ni errores JavaScript.


## Flujo de inicio personalizado

- [x] La cabecera de marca y la pantalla introductoria solo aparecen antes de iniciar la auditoría.
- [x] El nombre de empresa es el único campo de inicio y se utiliza en el resultado y la portada del PDF.
- [x] El campo de sector o actividad se ha eliminado.
- [x] El botón «Comenzar auditoría» permanece desactivado hasta que se introduce un nombre de empresa.
- [x] El cuestionario y la barra de progreso permanecen ocultos hasta pulsar «Comenzar auditoría».
- [x] Al terminar, el informe muestra el nombre de la empresa; al reiniciar, se vuelve a la portada y se conserva el nombre introducido.

## Ajustes de iconografía y composición según SVG originales

- [x] Se incorporan los tres archivos originales en `assets/iconos-auditoria.svg`, `assets/flor.svg` y `assets/linea.svg`.
- [x] La cabecera web y las cinco cabeceras del PDF usan `iconos-auditoria.svg`, sin reconstruir sus trazados a mano.
- [x] La flor de cierre de la página 5 procede de `flor.svg`.
- [x] La línea bicolor de la base del panel final procede de `linea.svg`.
- [x] El trazo junto al título de portada tiene una altura próxima al bloque tipográfico y está centrado verticalmente.
- [x] Los trazos de los subtítulos de sección son más cortos y se alinean con el texto.
- [x] Las etiquetas, puntuaciones y barras de las cinco dimensiones tienen más margen a ambos lados.
- [x] La lista de evidencias tiene más margen lateral sin eliminar elementos.
- [x] Los cuatro pasos de validación mantienen más separación vertical entre sus recuadros y sus frases.
- [x] La rasterización de SVG está optimizada para que el PDF de cinco páginas A4 pese menos de 1 MB.
- [x] Prueba real sobre GitHub Pages: SVG cargados, PDF de cinco páginas descargado, copyright y numeración presentes en todas las páginas y sin errores JavaScript ni desbordamiento móvil.

## Navegación de una pregunta por pantalla

- [x] Las 10 preguntas originales se conservan sin cambios.
- [x] Cada pantalla muestra exactamente una pregunta con sus opciones de respuesta.
- [x] Se mantienen las cinco secciones y su título descriptivo.
- [x] El indicador muestra la sección actual y la pregunta actual de 10.
- [x] El progreso avanza en incrementos del 10 % por pregunta.
- [x] La navegación anterior/siguiente conserva las respuestas y permite volver a una pregunta previa.
- [x] El diagnóstico y la generación del PDF siguen funcionando tras responder las 10 pantallas.
- [x] Prueba automatizada de escritorio y móvil: sin errores JavaScript ni desbordamiento horizontal.

## Revisión UX/UI de legibilidad y navegación

- [x] Texto explicativo de etapa: 17 px en escritorio y 16,5 px en móvil.
- [x] Texto de ayuda de preguntas: 15 px con interlineado de 1,65.
- [x] Opciones de respuesta: 16 px en escritorio y 15,5 px en móvil; área de selección mínima de 56 px.
- [x] Campos de texto: tamaño de fuente de 16 px y altura mínima de 48 px.
- [x] Enlace para saltar directamente al cuestionario.
- [x] Barra de progreso con semántica accesible y valor anunciado.
- [x] Al avanzar o retroceder, el foco se mueve al título de la etapa y el desplazamiento sigue el contenido activo.
- [x] Al terminar, el encabezado del diagnóstico recibe el foco y la introducción se oculta para priorizar el resultado.
- [x] Contraste mejorado para el texto de la cabecera y el botón principal de descarga.
- [x] Prueba automatizada con navegador: sin errores JavaScript, recorrido completo, tres recomendaciones y PDF de cinco páginas A4.
- [x] Prueba móvil a 390 px de ancho: sin desbordamiento horizontal.
- [ ] Revisión manual visual con diferentes dispositivos y una prueba con usuarios reales.

## Regresión visual del PDF rasterizado de referencia

Escenario de regresión utilizado para contrastar la distribución del PDF proporcionado:

- Q1=A, Q2=C, Q3=C, Q4=D, Q5=A, Q6=C, Q7=A, Q8=D, Q9=B, Q10=D.
- [x] El informe generado mantiene cinco páginas en formato A4.
- [x] La cabecera contiene el trío de iconos de marca en la portada y en las páginas 2 a 5, alineados en la misma posición.
- [x] Los círculos de los puntos del gráfico radial se conservan, tal como aparecen en la referencia.
- [x] Se conservan los paneles, barras de puntuación, cajas de recomendaciones, bandas de color, marca de agua y pies de página.
- [x] Las cinco páginas conservan el copyright y la numeración.
- [x] El texto extraído mantiene los títulos, párrafos y saltos de línea del plan de acción, sin texto que desborde el área de página.
- [x] Prueba automatizada sobre la web publicada: sin errores JavaScript.

## Aviso

Las pruebas automatizadas verifican la lógica implementada, no validan científicamente los perfiles. Los umbrales y los mensajes deben contrastarse con casos reales y ajustarse según los resultados de esa validación.
