【AI資格者が教える】Claudeで業務設計を高速化する要件定義書・詳細設計書・画面遷移図・ER図を“量産”するプロンプト集（Markdown版）
2026/06/27

# ✅ **GitHub 用 README（Markdown 完全版）**

```md
# Claude System Design Prompt Pack  
### 要件定義書・詳細設計書・画面遷移図・ER図を “自動生成” するプロンプト集（v4.2 PRO）

Claude を使って、業務設計ドキュメントを高速に生成するための  
**包括的なプロンプト集・テンプレート集・技術仕様書集** です。

このリポジトリでは、以下の技術文書を **100% Markdown で自動生成** できます。

- 要件定義書  
- 詳細設計書  
- 実装仕様書  
- 画面遷移図（UIフロー）  
- ER図（テキストベース）  
- デバッグ手順  
- 仕様変更手順  
- テスト方法  
- テスト結果レポート  
- CHANGELOG（バージョニング規約付き）  
- CR（変更依頼書）テンプレート  
- JSON スキーマ & 検証手順  

すべて **Claude に貼るだけで生成可能** です。

---

## 📁 ディレクトリ構成

```md
/
├── README.md
├── docs/
│   ├── 01_requirements.md
│   ├── 02_detail_design.md
│   ├── 03_implementation_spec.md
│   ├── 04_debugging.md
│   ├── 05_change_request.md
│   ├── 06_test_plan.md
│   ├── 07_test_report.md
│   ├── 08_changelog.md
│   └── 09_json_schema.md
└── prompts/
    ├── master_prompt.md
    ├── change_request_prompt.md
    ├── test_plan_prompt.md
    ├── test_report_prompt.md
    └── no_lie_prompt.md
```

---

## 🚀 使い方

### 1. Claude にプロンプトを貼る  
`/prompts/master_prompt.md` を Claude に貼るだけで、  
**要件定義 → 詳細設計 → 実装仕様 → テスト → バージョン管理**  
までを 1 本の Markdown に統合して生成します。

### 2. 仕様変更が発生したら  
`/prompts/change_request_prompt.md` を使用します。

### 3. 商用テスト時  
`/prompts/test_plan_prompt.md` を使用します。

### 4. テスト結果をまとめる  
`/prompts/test_report_prompt.md` を使用します。

### 5. 嘘をつかない技術文書を生成したいとき  
`/prompts/no_lie_prompt.md` を使用します。

---

# 🧪 **主要プロンプト（GitHub 用 Markdown）**

以下は GitHub に置くための **最適化済みプロンプト**。

---

## ① master_prompt.md（包括的技術仕様書生成）

```md
あなたは「技術仕様書の専門家」かつ「嘘をつかないAI」です。

以下の要件に基づき、実装（v4.2 PRO）に忠実な  
包括的な技術仕様書（Markdown）を1本にまとめて作成してください。

【含める内容】
1. 要件定義書
2. 詳細設計書
3. 実装仕様書
4. バグ発生時のデバッグ手順
5. 修正方法（仕様変更手順）
6. 商用テスト方法
7. テスト結果テンプレート
8. CHANGELOG（バージョニング規約付き）
9. CR（変更依頼書）テンプレート
10. JSONスキーマ（v4.2 PRO準拠）
11. JSON検証手順
12. 納品物一覧
13. すべてMarkdownで統合

【原則】
・推測禁止  
・未定義は未定義と書く  
・見出し階層は最大3階層  
・最後に「v4.2-PRO（YYYY-MM-DD）」を刻印
```

---

## ② change_request_prompt.md（仕様変更・CR対応）

```md
あなたは「仕様変更管理の専門家」です。

以下の技術仕様書（v4.2 PRO）をもとに、
仕様変更プロセス・CR・影響範囲分析・再テスト項目を作成してください。

【出力内容】
1. 仕様変更プロセス
2. CRテンプレート
3. 影響範囲分析
4. 修正後の再テスト項目
5. バージョンアップ規約（SemVer＋日付刻印）
```

---

## ③ test_plan_prompt.md（商用テスト）

```md
あなたは「QAエンジニア」です。

以下の実装（v4.2 PRO）に基づき、
商用テスト計画を作成してください。

【出力内容】
1. テスト目的
2. テスト観点
3. テストケース一覧
4. 合格基準
5. 不合格時の対応
6. バージョンアップ手順（PRO刻印）
```

---

## ④ test_report_prompt.md（テスト結果）

```md
あなたは「テスト結果レポートの専門家」です。

以下のテストケースに基づき、
テスト結果レポートを作成してください。

【出力内容】
1. 実行日
2. 実行者
3. 結果（Pass/Fail）
4. 不具合一覧
5. 修正内容
6. 再テスト結果
7. バージョン刻印
```

---

## ⑤ no_lie_prompt.md（100%嘘をつかない技術文書）

```md
あなたは「嘘をつかないAI」です。

以下の実装（v4.2 PRO）をもとに、
100%忠実な技術文書を作成してください。

【禁止事項】
・推測  
・存在しない仕様  
・曖昧な表現  

【許可される表現】
・未定義  
・仕様に記載なし  
・情報不足のため記述不可  

最後に  
v4.2-PRO（YYYY-MM-DD）  
を刻印してください。
```

---
