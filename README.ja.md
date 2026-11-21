# モグベビ｜離乳食の記録を、次の食事に活かす

**[English](./README.md) | 日本語**

### 何を食べたかだけでなく、どう食べたかも振り返れる離乳食管理

**Customer Discovery × Product Strategy × Requirements × AI Orchestration × Quality Management**

[App Storeでモグベビを見る](https://apps.apple.com/jp/app/id6823474417)

## 開発の背景｜食べたかどうかだけでは分からないこと

ステップ離乳食などの既存アプリは、食材の摂取チェックや離乳食の進行管理に便利です。一方で、食材の摂取有無を確認することが中心の画面構成や操作導線では、日々の食事を細かく記録・参照したい保護者にとって使いづらい場面があります。

- 以前よく食べた料理を、もう一度作りたい。
- どの程度の硬さや粒度なら食べやすかったか確認したい。
- 食後に症状が現れた際、その日の食事内容や体調を振り返りたい。
- 最近食べていない食材を確認し、次の献立を考えたい。

こうした判断には、食材の摂取有無だけでなく、食事内容や調理方法、子どもの反応などを日付・食事単位で簡単に記録し、必要なときに参照できることが重要です。

**食材のチェックだけでなく、日々の離乳食を記録し、次の食事に活かせるアプリへ。**

この課題から、記録時の操作負荷と情報の参照しやすさを重視した「モグベビ」を企画しました。食材記録、市販ベビーフードの商品検索、日記・カレンダー、摂取履歴などを組み合わせ、食事の振り返りと食材管理の双方を支援します。

## プロダクト概要

| 項目 | 内容 |
| --- | --- |
| **プロダクト** | 保護者向け離乳食・食材記録アプリ |
| **提供形態** | iOS／App Store公開 |
| **主な機能** | 食材記録、市販品検索、摂取履歴、最終摂取記録日・経過日数、食材の並び替え、保育施設準備 |
| **その他の機能** | 日記・カレンダー、「はじめて食べた」記録 |
| **担当領域** | 課題設定、プロダクト企画、要件定義、UX・優先順位判断、品質受入、公開承認 |
| **開発プロセス** | Claude Codeによる実装、ChatGPT/Codexによる別観点のレビュー、GitHub Issuesによる要求・変更管理 |

## 強みを示す4つのケーススタディ

### 01｜Customer Discovery — 困りごとを機能要件に変換

食材チェック中心の管理では対応しにくい、食事単位の記録・振り返りに着目。記録のしやすさと情報の参照性を設計上の重点としました。初期利用者の反応を踏まえ、最終摂取記録日・経過日数の表示と並び替えも追加しました。

**訴求能力：** Problem Framing、Requirements Translation、Prioritization

[Product Discoveryの詳細](./docs/ja/product-discovery.md)

### 02｜Product Leadership — 価値の伝え方も改善

当初のApp Store掲載は保育施設への入園準備が中心でした。しかし、日常の食材選びに役立つことが、より幅広い保護者にとっての価値になると判断。**記録を簡単に → 履歴を次の食材選びに活用 → 保育施設準備**という順に訴求を再設計しました。

**訴求能力：** Product Strategy、Positioning、UX、Scope Management

[Product Strategyの詳細](./docs/ja/product-and-launch.md)

### 03｜AI Orchestration — AIを実装手段として活用

人間が課題・要件・優先順位・採否を判断し、Claude Codeが実装、ChatGPT/Codexが別視点からレビュー。GitHub Issueを仕様の参照先とし、要求と修正の経緯を管理しました。

**訴求能力：** AI Orchestration、Requirements Management、Delivery Management

[AI Orchestrationの詳細](./docs/ja/delivery-governance.md)

### 04｜Quality Management — レビューを実際の品質改善へ

別AIのレビューで、**他アプリから移行した「初回摂取日」と「直近の摂取日」の混同**を検出。データの意味に合わせて表示・計算を修正し、境界ケースを回帰テストに追加しました。

**訴求能力：** Quality Management、Independent Review、Corrective Action

[Quality Managementの詳細](./docs/ja/quality-management.md)

## AIを活用したデリバリーモデル

```text
保護者に共通する日常的な困りごと
              ↓
解決すべき課題・価値の定義［Human］
              ↓
機能要件・優先順位の決定［Human］
              ↓
仕様・意思決定の管理［GitHub Issues］
              ↓
実装・検証［Claude Code］
              ↓
別AIによるレビュー・是正［ChatGPT/Codex + Claude Code］
              ↓
UX受入・リリース承認［Human］
              ↓
App Store公開
```

2026年10月には、食材履歴の改善とApp Store掲載の刷新を含むバージョン**1.0.1**を公開しました。これは実際の開発・意思決定プロセスの紹介であり、栄養状態や利用継続率などの改善を実証したという主張ではありません。

## 技術・ツール

**Product / Delivery:** 課題分析、要件定義、UX判断、GitHub Issues、リリース管理  
**AI:** Claude Code、ChatGPT/Codex

---

本リポジトリは公開可能な企画・デリバリー事例のみを掲載し、非公開の実装コードや個人情報は含めていません。
