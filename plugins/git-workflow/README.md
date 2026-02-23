# git-workflow

Git 操作に関するワークフローを提供するプラグイン。

## スキル

### commit

変更内容を分析し、関心事ごとにコミットを分割、Conventional Commits 形式のメッセージを提案して対話的にコミットする。

呼び出し: `/git-workflow:commit`

主な機能:

- staged / unstaged 両方の変更を対象とする
- 関心事が異なる変更は自動で分割を提案
- コミットメッセージ候補を3つ提示し、ユーザーが選択
- Co-Authored-By footer を自動付与
