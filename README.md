# <img src="assets/header.svg" alt="Roulette Server" width="400" style="display: block; margin-left: auto; margin-right: auto;">

## 🎲 ルーレットサーバー

このプロジェクトは、サイコロを振る機能を提供するModel Context Protocol (MCP) サーバーです。

### 🛠️ ツール

- **roll_dice**: 指定された数のサイコロを振ります。

  - **入力**:
    - `diceCount`: 振るサイコロの数 (1から10までの整数)。
  - **出力**:
    - 振られたサイコロの目の結果。

### ⚙️ インストール

1.  このリポジトリをクローンします。
   ```bash
   git clone [リポジトリURL]
   ```
2.  `roulette-server`ディレクトリに移動します。
   ```bash
   cd roulette-server
   ```
3.  依存関係をインストールします。
   ```bash
   npm install
   ```
4.  サーバーをビルドします。
   ```bash
   npm run build
   ```
5.  サーバーを実行します。
   ```bash
   node build/index.js
   ```

### 📝 使用例

MCPクライアントを使用して、`roll_dice`ツールを呼び出すことでサイコロを振ることができます。

例:

```json
{
  "tool": "roll_dice",
  "arguments": {
    "diceCount": 3
  }
}
```

### 📜 コミットメッセージ形式

コミットメッセージは以下の形式に従うこと:

```
<絵文字> <タイプ>: <タイトル>
<本文>
<フッター>
```

- タイトル（コミットメッセージの1行目）の先頭には必ず絵文字を付与し、日本語で記述すること。
- タイプは以下のいずれかとする：
  - **feat**: 新機能
  - **fix**: バグ修正
  - **docs**: ドキュメントの変更
  - **style**: コードスタイルの変更（動作に影響しない）
  - **refactor**: リファクタリング
  - **perf**: パフォーマンス改善
  - **test**: テストの追加・修正
  - **chore**: ビルドプロセスやツールの変更

### 📄 ライセンス

このプロジェクトはMITライセンスの下で公開されています。
