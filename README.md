# isasaka-plugins

個人用の Claude Code プラグインマーケットプレイス。

## マーケットプレイスの追加

```
/plugin marketplace add <このリポジトリのURL>
```

## プラグイン一覧

| プラグイン | 説明 |
|-----------|------|
| [git-workflow](./plugins/git-workflow/) | Git 操作に関するワークフローを提供するプラグイン |

## プラグインのインストール

マーケットプレイス追加後、個別のプラグインをインストールする:

```
/plugin install git-workflow@isasaka-plugins
```

## 新規プラグインの作成

1. `plugins/<プラグイン名>/` ディレクトリを作成
2. `.claude-plugin/plugin.json` に `name`, `description`, `version` を記載
3. `skills/`, `commands/`, `agents/`, `hooks/` に必要なファイルを配置
4. `.claude-plugin/marketplace.json` の `plugins` 配列に追加

## ディレクトリ構成

```
.claude-plugin/
  marketplace.json          # マーケットプレイス定義
plugins/
  git-workflow/             # git-workflow プラグイン
    .claude-plugin/
      plugin.json
    skills/
      commit/
        SKILL.md
    README.md
```

## 参考資料

- [Plugins](https://docs.claude.com/en/docs/claude-code/plugins)
- [Plugins reference](https://docs.claude.com/en/docs/claude-code/plugins-reference)
- [Plugin marketplaces](https://docs.claude.com/en/docs/claude-code/plugin-marketplaces)
- [スラッシュコマンド](https://docs.claude.com/ja/docs/claude-code/slash-commands)
- [サブエージェント](https://docs.claude.com/ja/docs/claude-code/sub-agents)
- [MCP](https://docs.claude.com/ja/docs/claude-code/mcp)
- [Hooks](https://docs.claude.com/ja/docs/claude-code/hooks-guide)
