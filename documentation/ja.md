<!-- ELUCENIA technical documentation · has-bled · ja · no clinical/professional/rights approval -->

# HAS-BLED

[条件・出典・許諾](https://elucenia.org/ja/tools/has-bled)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 管理不良の高血圧（収縮期血圧 \> 160 mmHg）

`h`

### 腎機能異常（透析、移植またはクレアチニン ≥ 2.26 mg/dL）

`rim`

### 肝機能異常（肝硬変、またはビリルビン \> 基準値の2×かつAST/ALT \> 3×）

`fig`

### 脳卒中の既往

`avc`

### 出血の既往または素因（貧血・血小板減少）

`sang`

### 不安定なINR（治療域内時間 \< 60%）

`inr`

### 年齢 \> 65 歳

`idoso`

### 抗血小板薬または抗炎症薬

`drogas`

### 飲酒（週 ≥ 8杯）

`alcool`

## 方法の版

HAS-BLED/Pisters 2010：9点；腎/肝/薬物/飲酒を別々に計点；ESC 2024文脈

## 記載された計算式

各1点：H高血圧，A腎/肝異常（各1），S脳卒中，B出血，LINR不安定，E高齢（\> 65），D薬物/飲酒（各1）。最大：9。

## 限界・対象集団

原HAS-BLEDは、心房細動における一年以内の大出血を推定します。合計点は自動的に抗凝固の禁忌を表すものではありません。因子の定義と現代の指針は版に対応する必要があります。集団の較正と抗血栓治療が、その解釈に影響します。

## 参考文献

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

高出血リスク

| 結果の詳細 | |
| --- | --- |
| 大出血 | 100患者年あたり12.50以上 |

修正可能な因子：血圧をコントロールし、INRを安定させるかDOACへ変更、抗血小板薬/NSAIDsを見直し、飲酒を減らす。


### 2

高出血リスク

| 結果の詳細 | |
| --- | --- |
| 大出血 | 3.74 / 100患者年 |

修正可能な因子：血圧をコントロールする。


### 3

出血リスクが低い

| 結果の詳細 | |
| --- | --- |
| 大出血 | 1.13 / 100患者年 |

