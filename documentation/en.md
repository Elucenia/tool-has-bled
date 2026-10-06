<!-- ELUCENIA technical documentation · has-bled · en · no clinical/professional/rights approval -->

# HAS-BLED

[conditions, sources and permissions](https://elucenia.org/en/tools/has-bled)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Uncontrolled hypertension (systolic blood pressure \> 160 mmHg)

`h`

### Abnormal renal function (dialysis, transplant or creatinine ≥ 2.26 mg/dL)

`rim`

### Abnormal liver function (cirrhosis or bilirubin \> 2× and AST/ALT \> 3× normal)

`fig`

### Previous stroke

`avc`

### Prior bleeding or predisposition (anemia, thrombocytopenia)

`sang`

### Labile INR (time in therapeutic range \< 60%)

`inr`

### Age \> 65 years

`idoso`

### Antiplatelet or anti-inflammatory medication

`drogas`

### Alcohol (≥ 8 drinks per week)

`alcool`

## Method edition

HAS-BLED/Pisters 2010: 9 points; renal/liver/drugs/alcohol separate; ESC 2024 context

## Documented formula

One point each: Hypertension, Abnormal renal/liver function (1 each), Stroke, Bleeding, Labile INR, Elderly (\> 65), Drugs/alcohol (1 each). Maximum: 9.

## Limits and population

The original HAS-BLED estimates major bleeding within one year in atrial fibrillation. The total is not an automatic contraindication to anticoagulation; factor definitions and contemporary guidance must match the version. Population calibration and antithrombotic treatment affect its interpretation.

## References

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

High bleeding risk

| Result details | |
| --- | --- |
| Major bleeding | 12.50 or more per 100 patient-years |

Modifiable factors: control blood pressure, stabilize INR or switch to DOAC, review antiplatelets/NSAIDs, reduce alcohol.


### 2

High bleeding risk

| Result details | |
| --- | --- |
| Major bleeding | 3.74 per 100 patient-years |

Modifiable factors: control blood pressure.


### 3

Low bleeding risk

| Result details | |
| --- | --- |
| Major bleeding | 1.13 per 100 patient-years |

