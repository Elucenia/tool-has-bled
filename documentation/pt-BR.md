<!-- ELUCENIA technical documentation · has-bled · pt-BR · no clinical/professional/rights approval -->

# HAS-BLED

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/has-bled)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Hipertensão não controlada (PAS \> 160 mmHg)

`h`

### Função renal alterada (diálise, transplante ou creatinina ≥ 2,26 mg/dL)

`rim`

### Função hepática alterada (cirrose ou bilirrubina \> 2× e AST/ALT \> 3× o normal)

`fig`

### AVC prévio

`avc`

### Sangramento prévio ou predisposição (anemia, plaquetopenia)

`sang`

### INR lábil (tempo na faixa terapêutica \< 60%)

`inr`

### Idade \> 65 anos

`idoso`

### Antiagregante ou anti-inflamatório

`drogas`

### Álcool (≥ 8 doses por semana)

`alcool`

## Edição do método

HASBLED/Pisters 2010:9 pontos; renal/hepático/drogas/álcoolseparados; contexto ESC 2024

## Fórmula documentada

Um ponto para cada item: Hipertensão, função renal/hepática Alterada (1 cada), Stroke (AVC), Bleeding (sangramento), Labile INR, Elderly (\> 65), Drugs/álcool (1 cada). Máximo: 9.

## Limites e população

O HAS-BLED original estima sangramento maior em um ano em fibrilação atrial. O total não representa contraindicação automática à anticoagulação; definições dos fatores e orientação contemporânea devem corresponder à versão. A calibração e o tratamento antitrombótico da população influenciam sua interpretação.

## Referências

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Alto risco de sangramento

| Detalhes do resultado | |
| --- | --- |
| Sangramento maior | 12,50 ou mais por 100 pacientes-ano |

Fatores modificáveis: controlar a pressão, estabilizar o INR ou trocar por DOAC, rever antiagregantes/AINEs, reduzir o álcool.


### 2

Alto risco de sangramento

| Detalhes do resultado | |
| --- | --- |
| Sangramento maior | 3,74 por 100 pacientes-ano |

Fatores modificáveis: controlar a pressão.


### 3

Risco de sangramento baixo

| Detalhes do resultado | |
| --- | --- |
| Sangramento maior | 1,13 por 100 pacientes-ano |

