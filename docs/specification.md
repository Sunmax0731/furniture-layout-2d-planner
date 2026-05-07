# 仕様

        ## 対象レコード

        - `room`
- `furniture`
- `layoutCandidate`
- `clearanceCheck`

        ## 必須項目

        `title`, `roomSize`, `itemSize`

        ## 警告項目

        `clearanceNote`, `reviewDate`

        ## フロー

        1. 入力レコードを受け取る。
        2. `src/core/scenarioEngine.js` が必須項目と警告項目を評価する。
        3. `src/report/reportBuilder.js` が検証結果を集計する。
        4. `dist/validation-result.json` を release evidence の前提証跡にする。

        ## 保存方針

        間取りと家具寸法のみをブラウザ内で扱い、位置情報や個人情報を扱わない
