# shutx-apm

`shutx-skills` パッケージ。AI Agent 用の skills を APM (Agent Package Manager) 形式で配布します。

## Install

```bash
apm install
```

主なオプション:

| オプション | 説明 |
|-----------|------|
| `--target, -t` | 配置先ハーネスを指定（カンマ区切り）。例: `-t claude,copilot`。指定可能値: `claude`, `copilot`, `cursor`, `opencode`, `codex`, `gemini`, `windsurf`, `agent-skills`, `vscode`, `all` |
| `--parallel-downloads <N>` | 同時ダウンロード数の上限（デフォルト: 4、`0` で無効化） |
| `--dev` | dev dependencies も含めて配置（authoring 用） |
| `--force` | 衝突時にローカルファイルを上書き |

詳細は [公式 CLI Commands](https://microsoft.github.io/apm/reference/cli-commands/) を参照。

## Skills

- [`create-doc-for-job-hunt`](./.apm/skills/create-doc-for-job-hunt/SKILL.md)

## 公式

[APM (Microsoft)](https://microsoft.github.io/apm/)
