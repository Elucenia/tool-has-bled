<!-- ELUCENIA technical documentation · has-bled · es · no clinical/professional/rights approval -->

# HAS-BLED

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/has-bled)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Hipertensión no controlada (presión arterial sistólica \> 160 mmHg)

`h`

### Función renal alterada (diálisis, trasplante o creatinina ≥ 2,26 mg/dL)

`rim`

### Función hepática alterada (cirrosis o bilirrubina \> 2× y AST/ALT \> 3× el valor normal)

`fig`

### Ictus previo

`avc`

### Sangrado previo o predisposición (anemia, trombocitopenia)

`sang`

### INR lábil (tiempo en rango terapéutico \< 60%)

`inr`

### Edad \> 65 años

`idoso`

### Antiagregante o antiinflamatorio

`drogas`

### Alcohol (≥ 8 consumiciones por semana)

`alcool`

## Edición del método

HAS-BLED/Pisters 2010: 9 puntos; renal/hepático/fármacos/alcohol separados; contexto ESC 2024

## Fórmula documentada

Un punto cada uno: H hipertensión, A alteración renal/hepática (1 cada), S ictus, B sangrado, L INR lábil, E edad (\> 65), D fármacos/alcohol (1 cada). Máximo: 9.

## Límites y población

El HAS-BLED original estima el sangrado mayor en un año en fibrilación auricular. El total no representa una contraindicación automática para la anticoagulación; las definiciones de los factores y la orientación contemporánea deben corresponder a la versión. La calibración y el tratamiento antitrombótico de la población influyen en su interpretación.

## Referencias

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
