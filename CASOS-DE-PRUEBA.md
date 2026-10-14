# Casos de prueba manuales

Estos escenarios son regresiones mínimas para comprobar que las reglas de perfil y el informe se mantienen coherentes después de cambiar el cuestionario o la puntuación.

| Caso | Respuestas relevantes | Resultado esperado |
|---|---|---|
| Marca consolidada | Todas A; Q9 = E | Marca consolidada, puntuación 100/100 y tres recomendaciones de optimización. |
| Marca desalineada | Q3 = D; resto A | Marca desalineada; el índice global se limita por la debilidad crítica. |
| Marca en construcción | Q1 = D y Q2 = D; resto A | Marca en construcción; no se oculta la falta de fundamentos con una media alta. |
| Marca dispersa | Q5 = D y Q6 = D; resto A | Marca dispersa; coherencia es la dimensión crítica. |
| Marca funcional | Q7 = C y Q8 = C; resto A | Marca funcional; diferenciación y personalidad son la principal debilidad. |
| Caso mixto con empate | Todas B; Q9 = B | Marca dispersa como desempate secundario declarado; no se usa construcción por defecto. |
| Diferenciación débil | Q7 = D y Q8 = A; resto A | Marca funcional; índice ajustado máximo de 74 por una dimensión por debajo de 60. |

## Verificaciones funcionales

- [x] El código JavaScript pasa `node --check`.
- [x] Los cinco perfiles se activan en escenarios diseñados para ellos.
- [x] Cada escenario de resultado muestra tres recomendaciones.
- [x] La web pública genera un PDF de cinco páginas A4 con el gráfico radial de cinco dimensiones.
- [x] Navegación de escritorio y flujo completo en móvil verificados con navegador automatizado.
- [x] No se registraron errores JavaScript durante estas pruebas.
- [x] GitHub Pages está publicado y la URL pública se ha probado directamente.
- [ ] Revisar el diseño visual del PDF y validarlo con empresas reales antes del lanzamiento comercial.

## Revisión de paleta visual

- [x] Carbón `#29272A` sustituye al verde oscuro en los bloques y botones principales.
- [x] Fondo marfil `#F5F2ED` aplicado al fondo general y blanco cálido `#FFFEFC` a las tarjetas.
- [x] Terracota `#C57A52` y terracota oscuro `#96563B` aplicados a acentos, progresión, selección y CTA.
- [x] Salvia grisácea `#9AA397` reservada para indicadores y gráficos.
- [x] PDF adaptado a la misma paleta.
- [x] Navegador automatizado sobre la URL pública: comprobados los colores calculados y descarga de PDF de cinco páginas A4.

## Flujo de inicio personalizado

- [x] La cabecera de marca y la pantalla introductoria solo aparecen antes de iniciar la auditoría.
- [x] El nombre de empresa es el único campo de inicio y se utiliza en el resultado y la portada del PDF.
- [x] El campo de sector o actividad se ha eliminado.
- [x] El botón «Comenzar auditoría» permanece desactivado hasta que se introduce un nombre de empresa.
- [x] El cuestionario y la barra de progreso permanecen ocultos hasta pulsar «Comenzar auditoría».
- [x] Al terminar, el informe muestra el nombre de la empresa; al reiniciar, se vuelve a la portada y se conserva el nombre introducido.

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

## Aviso

Las pruebas automatizadas verifican la lógica implementada, no validan científicamente los perfiles. Los umbrales y los mensajes deben contrastarse con casos reales y ajustarse según los resultados de esa validación.
