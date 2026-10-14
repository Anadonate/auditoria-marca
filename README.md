# Auditoría de Marca Visual · Ana Donate

Prototipo independiente del proyecto `diagnostico-marca`. Este repositorio no modifica el diagnóstico anterior.

## Qué incluye

- Cuestionario guiado de 10 preguntas cerradas, agrupadas en cinco etapas.
- Nombre de empresa y sector opcionales para personalizar el informe.
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

## Modelo de evaluación

Consulta [CRITERIOS-EVALUACION.md](./CRITERIOS-EVALUACION.md) para ver la escala, los pesos, las reglas de perfiles y las limitaciones del resultado.

## Nota profesional

El resultado es una autoevaluación orientativa basada en respuestas declaradas, no una auditoría directa de materiales, una investigación con clientes ni un análisis de competencia. Antes de utilizarlo como herramienta comercial definitiva, conviene hacer pruebas con combinaciones de respuestas y contrastar el resultado con marcas reales.
