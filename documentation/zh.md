<!-- ELUCENIA technical documentation · has-bled · zh · no clinical/professional/rights approval -->

# HAS-BLED

[条件、来源与许可](https://elucenia.org/zh/tools/has-bled)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 未控制的高血压（收缩压 \> 160 mmHg）

`h`

### 肾功能异常（透析、移植或肌酐 ≥ 2.26 mg/dL）

`rim`

### 肝功能异常（肝硬化或胆红素 \> 正常值的 2× 且 AST/ALT \> 3×）

`fig`

### 既往卒中

`avc`

### 既往出血或出血倾向（贫血、血小板减少）

`sang`

### INR 不稳定（治疗范围内时间 \< 60%）

`inr`

### 年龄 \> 65 岁

`idoso`

### 抗血小板药或抗炎药

`drogas`

### 饮酒（每周 ≥ 8 份）

`alcool`

## 方法版本

HAS-BLED/Pisters 2010：9分；肾/肝/药物/酒精分别；ESC 2024背景

## 已记录的公式

每项一分：H高血压、A肾/肝功能异常（各1）、S卒中、B出血、LINR不稳定、E年龄（\> 65）、D药物/酒精（各1）。最高：9。

## 限制与适用人群

原始HAS-BLED估计心房颤动患者一年内的大出血风险。总分不自动构成抗凝禁忌证；因素定义及当前指导须与版本一致。人群的校准和抗血栓治疗会影响其解释。

## 参考文献

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
