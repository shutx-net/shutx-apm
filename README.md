# shutx-apm

`shutx-skills` パッケージ。Claude 用の skills を APM (Agent Package Manager) 形式で配布します。

## 概要

詳細は [AGENTS.md](AGENTS.md) を参照してください。

## 含まれる Skills

### `create-doc-for-job-hunt`

就職活動用書類（履歴書 / 職務経歴書 / エントリーシート）を HTML/CSS で生成する Claude Skill。

- パス: [`.apm/skills/create-doc-for-job-hunt/`](./.apm/skills/create-doc-for-job-hunt/)
- 詳細: [SKILL.md](./.apm/skills/create-doc-for-job-hunt/SKILL.md)

#### 特徴

- HTML/CSS のみで構成（JavaScript 不要、Live Server で即確認可能）
- A4 / B5 / US Letter 等の用紙サイズ・縦横向きをユーザーが指定
- `japanese-formal` / `modern-simple` の 2 デザインスタイル
- PDF 化を見据えた CSS（`@page` ルール、mm 単位、改ページ制御）

## ディレクトリ構造

```
.
├── apm.yml                          # APM 設定
├── AGENTS.md                        # パッケージ概要
├── CLAUDE.md                        # Claude 用プロジェクトルール
└── .apm/
    └── skills/
        └── create-doc-for-job-hunt/
            ├── SKILL.md
            ├── references/
            └── templates/
```

## 公式

[APM (Microsoft)](https://microsoft.github.io/apm/)
