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
- [x] La descarga genera un PDF de cinco páginas A4 e incluye un gráfico radial con las cinco dimensiones.
- [x] Navegación de escritorio y flujo completo en móvil verificados con navegador automatizado.
- [x] No se registraron errores JavaScript durante estas pruebas.
- [ ] Activar GitHub Pages y comprobar la URL pública una vez publicada.
- [ ] Revisar el diseño visual del PDF y validarlo con empresas reales antes del lanzamiento comercial.

## Aviso

Las pruebas automatizadas verifican la lógica implementada, no validan científicamente los perfiles. Los umbrales y los mensajes deben contrastarse con casos reales y ajustarse según los resultados de esa validación.
