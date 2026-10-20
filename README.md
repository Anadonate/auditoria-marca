# Auditoría de Marca Visual · Ana Donate

Prototipo independiente del proyecto `diagnostico-marca`. Este repositorio no modifica el diagnóstico anterior.

## Identidad visual

La interfaz y el PDF utilizan una paleta alineada con la identidad visual de Ana Donate:

- Carbón `#29272A`: encabezados, bloques principales y botones primarios.
- Marfil `#F5F2ED`: fondo general y lectura del formulario.
- Blanco cálido `#FFFEFC`: tarjetas y superficies.
- Rosa EA `#EA5A77`: progreso, selección, acentos y detalles gráficos; también marca acciones principales.
- Verde EA `#46B382`: estados interactivos, contornos e indicadores gráficos.
- Dorado EA `#D2A158`: barras de dimensión, detalles y elementos decorativos.
- El marfil de fondo `#F5F2ED` y el carbón `#29272A` se mantienen. El dorado se reserva para elementos gráficos; los textos pequeños se muestran en carbón para preservar el contraste.
- Gris cálido `#716D6D`: texto secundario.

La cabecera inicial y el campo de nombre solo aparecen antes de comenzar; al iniciar, la cabecera desaparece y el cuestionario pasa a primer plano. La tipografía explicativa se ha ampliado y la navegación mueve el foco al encabezado de la etapa activa. Los estados hover de las respuestas usan el dorado EA, y los símbolos flor, diana y cursor sustituyen los puntos decorativos en la web y el informe. Los controles tienen áreas táctiles más cómodas, se conserva la preferencia de movimiento reducido y el formulario no debe provocar desplazamiento horizontal en móvil.


## Cuestionario y PDF

- La pregunta 9 tiene cuatro opciones, alineadas con las demás preguntas; el cuestionario mantiene sus 10 preguntas.
- El PDF personalizado consta de cinco páginas A4. La portada usa paneles rosa pálido y blanco cálido sobre carbón; las páginas interiores comparten la paleta EA.
- El gráfico radial se dibuja a partir de las cinco puntuaciones calculadas para cada respuesta, de modo que la forma cambia en cada diagnóstico.
- Las recomendaciones y las listas de validación usan una numeración más clara, con texto legible, mayor contraste y acentos rosa, dorado y verde.


## Legibilidad del cuestionario

El formulario conserva 10 preguntas, presentadas una por pantalla, con cuatro respuestas cerradas cada una. Se han retirado las frases auxiliares bajo cada pregunta para reducir la carga de lectura, manteniendo las descripciones introductorias de las cinco secciones. En móvil, el aviso de privacidad queda a 28 px del borde superior del pie de página y el bloque de recomendaciones del informe conserva 20 px de separación respecto al diagnóstico.

## Qué incluye

- Cuestionario guiado de 10 preguntas cerradas, presentadas una por pantalla y agrupadas en cinco secciones. La navegación y el progreso avanzan pregunta a pregunta.
- Pantalla de inicio independiente con nombre de empresa obligatorio para personalizar la portada del informe; se ha eliminado el campo de sector.
- Cinco dimensiones con un índice ponderado de desarrollo de marca.
- Asignación explicada a uno de cinco perfiles: Marca en construcción, Marca dispersa, Marca funcional, Marca consolidada o Marca desalineada.
- Tres recomendaciones derivadas de las dimensiones y respuestas seleccionadas.
- Exportación de un PDF de varias páginas que se genera localmente en el navegador.
- Diseño responsive y tratamiento de las respuestas dentro del navegador; este prototipo no envía respuestas a un servidor.

## Ejecutar y publicar

La web está hecha con HTML, CSS y JavaScript sin proceso de compilación. Para probarla localmente, abre `index.html` en un navegador con conexión a internet (las fuentes y jsPDF se cargan desde CDN).

Para publicar con GitHub Pages:

1. Abre **Settings → Pages** en este repositorio.
2. En **Build and deployment**, selecciona **Deploy from a branch**.
3. Selecciona la rama `main` y la carpeta `/ (root)`, y guarda.
4. Espera a que termine la publicación. La URL prevista es https://anadonate.github.io/auditoria-marca/.


## Informe final y PDF

- Resultado web con cabecera carbón, iconos de EA, puntuación destacada y tarjetas con mayor jerarquía tipográfica.
- Gráfico radial de cinco dimensiones en pantalla con escala, iconos de marca y leyenda numérica accesible.
- Recomendaciones, fortalezas y áreas de atención en paneles con fondo claro, borde suave y acentos rosa/dorado/verde.
- PDF de cinco páginas A4 con portada carbón, marca gráfica, títulos y marcadores coherentes con la paleta EA; las páginas interiores usan fondo marfil y barras de puntuación por nivel.

## Modelo de evaluación

Consulta [CRITERIOS-EVALUACION.md](./CRITERIOS-EVALUACION.md) para ver la escala, los pesos, las reglas de perfiles y las limitaciones del resultado.

## Nota profesional

El resultado es una autoevaluación orientativa basada en respuestas declaradas, no una auditoría directa de materiales, una investigación con clientes ni un análisis de competencia. Antes de utilizarlo como herramienta comercial definitiva, conviene hacer pruebas con combinaciones de respuestas y contrastar el resultado con marcas reales.
