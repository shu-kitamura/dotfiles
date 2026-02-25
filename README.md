# dotfiles

このリポジトリは、シェル設定などの dotfiles を管理するためのものです。
主に `.bashrc` などの設定ファイルを保存し、必要に応じて配置・更新します。

## 含まれるもの
- `bash/`: Bash 関連の設定ファイル

## 使い方
1. このリポジトリを任意の場所にクローンします。
2. 必要な設定ファイルを手動で配置するか、シンボリックリンクを作成してください。

例:
```bash
ln -s "$(pwd)/bash/.bashrc" ~/.bashrc
```

## 注意事項
- 既存の設定ファイルを上書きする前にバックアップを取ってください。
- 環境によって必要な設定が異なる場合は、ローカルで適宜調整してください。


## Codex 設定メモ
- `.codex/config.toml` は `web_search = "live"` を使う形式に更新しています（旧 `features.web_search*` は非推奨）。
- `playwright` / `next-devtools` MCP は `npx -y ...@latest` と `startup_timeout_sec` を設定し、初回起動時の失敗を減らしています。
