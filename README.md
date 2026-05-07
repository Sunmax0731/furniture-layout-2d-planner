# furniture-layout-2d-planner

家具配置2Dプランナー は、部屋寸法と家具寸法だけで配置案を比較する静的Webプランナーです。

## Closed Alpha Scope

- Rank: 23
- Tier / Score: P1 / 64
- Domain / Idea No: WebApp / 7
- 主な公開先: GitHub Pages / GitHub Release
- GitHub: https://github.com/Sunmax0731/furniture-layout-2d-planner
- Prerelease: https://github.com/Sunmax0731/furniture-layout-2d-planner/releases/tag/v0.1.0-alpha.1

## 実装概要

- `src/core`: 製品プロファイルと代表シナリオ評価
- `src/validators`: 期待結果検証
- `src/report`: 検証レポート生成
- `src/review-model`: レビューゲートと責務モデル
- `src/cli`: `samples/representative-suite.json` の自動検証

## 代表データ

`samples/representative-suite.json` は `happy-path`、`missing-required`、`warning`、`mixed-batch` を含みます。

## 検証

```powershell
cd D:\AI\WebApp\furniture-layout-2d-planner
cmd.exe /d /s /c npm test
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` を参照してください。
