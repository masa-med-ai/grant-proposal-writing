# 12. MCP 導入確認シート

> Step1-2, 1-3 の作業ログ。Claude はツール一覧をチェックし、欠けていればユーザーに導入推奨を伝える。

## 1. KAKEN MCP

- [ ] `mcp__KAKEN_Search__*` 系ツールが利用可能（例：`kaken_search_projects`, `kaken_search_researchers`, `kaken_get_project`, `kaken_get_researcher_grants`）

### 未導入時のユーザー案内テンプレート

```
KAKENHI（科研費データベース）を検索するためのMCPが未導入です。
過去の採択課題を確認することで、自分の研究テーマの新規性・被りを
チェックできるため、本PJTでは導入を強く推奨します。

【導入手順】
1. Bundleファイルをダウンロード
   https://github.com/masa-med-ai/KAKENHI-search-mcpbundle

2. Cinii APIキーを取得
   https://api.ci.nii.ac.jp/ja/
   ※ 申請から発行まで数営業日かかる場合があります

3. Claudeにbundleをインストール（READMEに従う）
```

### 確認結果
- 検出されたツール: _____________________
- アクション: ☐ 既に導入済み ☐ ユーザーに導入推奨済み ☐ ユーザーがスキップを選択

## 2. PubMed MCP

- [ ] PubMed検索系ツールが利用可能（例：`search`, `fetch`, `count`, `find_similar_articles`）

### 未導入時のユーザー案内テンプレート

```
PubMed検索用MCPが未導入です。本PJTでは国内外の研究動向確認や
引用文献収集に必須のため、導入を強く推奨します。

【導入手順】
Claude Codeのプラグインマーケットプレイスから "pubmed" を検索して
インストールしてください。
```

### 確認結果
- 検出されたツール: _____________________
- アクション: ☐ 既に導入済み ☐ ユーザーに導入推奨済み ☐ ユーザーがスキップを選択

## 3. Step1-2, 1-3 完了サマリー

- KAKEN MCP: ☐ 利用可能 ☐ 未導入（次工程に影響あり）
- PubMed MCP: ☐ 利用可能 ☐ 未導入（次工程に影響あり）
- 次のアクション: テーマ壁打ち（Step1-4）へ進む
