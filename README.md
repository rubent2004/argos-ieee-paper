# Paper IEEE de ArGos

## Archivos

- `main.tex`: manuscrito en inglés con formato `IEEEtran` para conferencia.
- `references.bib`: 17 referencias utilizadas, seleccionadas de los 20 PDFs
  recuperados en `Paper/Recursos/`.
- `source-selection.md`: justificación de fuentes incluidas y descartadas.
- `build/main.pdf`: salida local de compilación.
- `../../output/pdf/argos-ieee-paper.pdf`: copia estable para entrega.

## Compilación

Desde esta carpeta:

```bash
uv run python -B \
  /home/ruben/.agents/skills/latex-paper-en/scripts/compile.py \
  main.tex --outdir build
```

## Supuestos editoriales

- Idioma: inglés, siguiendo el tono del paper de ejemplo suministrado.
- Formato: IEEE conference, A4, dos columnas.
- Autor actual: Rubén Torres. Antes de enviar, se deben confirmar afiliación,
  correo, orden de autores y contribuciones de cualquier coautor.
- Longitud actual: seis páginas, referencias incluidas.
- Tipo de contribución: paper de sistema y artefacto. No afirma superioridad de
  detección ni usa las capturas de demostración como resultados experimentales.

## Antes de someterlo

El manuscrito deja explícitos los experimentos aún pendientes: evaluación
longitudinal sobre targets propios, precisión/verificación de hallazgos,
benchmark MCP dirigido por tareas, prompt injection y pruebas con APIs reales.
También se debe revisar la política de la conferencia sobre el uso de IA y hacer
la divulgación correspondiente cuando la sede lo exija.
