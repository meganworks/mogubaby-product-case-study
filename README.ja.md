# モグベビ｜離乳食の「食べた記録」を、日々の判断に活かす

**[English](./README.md) | 日本語**

### 市販ベビーフードの記録から、食材の摂取履歴・保育施設の準備まで

**Customer Discovery × Product Strategy × Requirements × AI Orchestration × Quality Management**

[App Storeでモグベビを見る](https://apps.apple.com/jp/app/id6823474417)

## 開発の背景｜既存の食材チェックだけでは残る手間

離乳食アプリには、食材ごとの「食べた／まだ」をチェックできるものがあります。それでも、市販のベビーフードを使う場面では、**商品に含まれる食材のうち、実際に口にしたものを記録する**作業が発生します。さらに、「最後にいつ食べたか」を思い出したり、保育施設から指定された食材の摂取状況を確認したりするために、過去の記録を何度も見返すことがあります。

**「市販品を使った日の記録が、その後の食材選びや保育施設の準備にも、そのまま役立つようにできないか」**

モグベビでは、ベビーフードの商品名から含有食材を呼び出し、**実際に食べた食材を確認して記録**できます。その履歴をもとに、食材ごとの最終記録日・経過日数を確認し、保育施設の指定食材の摂取状況もチェックできます。

既存の大手アプリにも食材チェックやベビーフードの記録機能はあります。モグベビが重視したのは、未提供機能の数ではなく、**商品単位の食事記録から、食材単位の履歴確認・次の行動までをつなぐ一連の操作**です。

## プロダクト概要

| 項目 | 内容 |
| --- | --- |
| **プロダクト** | 保護者向け離乳食・食材記録アプリ |
| **提供形態** | iOS／App Store公開 |
| **主な機能** | 食材記録、市販品検索、摂取履歴、最終摂取記録日・経過日数、食材の並び替え、保育施設準備 |
| **その他の機能** | 「はじめて食べた」記録、日記などの成長記録 |
| **担当領域** | 課題設定、プロダクト企画、要件定義、UX・優先順位判断、品質受入、公開承認 |
| **開発プロセス** | Claude Codeによる実装、ChatGPT/Codexによる別観点のレビュー、GitHub Issuesによる要求・変更管理 |

## 強みを示す4つのケーススタディ

### 01｜Customer Discovery — 困りごとを機能要件に変換

離乳食管理の課題は「記録を残すこと」だけではありません。**残した記録を日々の判断に使いたい**というニーズに着目し、初期利用者の反応から、最終摂取記録日・経過日数の表示と並び替えを優先。献立の自動生成などへスコープを拡張せず、必要な改善に絞りました。

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

**目指したこと：** *困りごとを発見し、必要な価値を定義する。技術やAIを手段として、利用者に届くプロダクトへ変換する。*

本リポジトリは公開可能な企画・デリバリー事例のみを掲載し、非公開の実装コードや個人情報は含めていません。
