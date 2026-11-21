# Requirements Management｜AI活用型デリバリー統制

[ポートフォリオ](../../README.ja.md) ・ [English](../en/delivery-governance.md)

## GitHub Issueを仕様の正本として管理

GitHub Issueには、最新版の要求、スコープ、受入条件、レビュー指摘、対応履歴を集約しました。ユーザーの反応に応じて優先順位を変更する際も、従来案を無言で変更せず、何を上書きするか明示しています。

## 役割分担

| 担当 | 責任範囲 |
| --- | --- |
| Human Product Owner | 課題設定、優先順位、UX判断、機能範囲、リリース承認 |
| Claude Code | 機能・クリエイティブ実装、技術的修正、テスト実行・報告 |
| ChatGPT / Codex | 異なる視点からの独立レビュー、境界ケースの指摘 |
| GitHub Issues | 要件・判断・レビュー・是正措置のトレーサビリティ |
| CI・テスト | 特定の変更に対する自動検証。レビューと実行結果は区別 |

## 具体例

食材履歴の新機能とApp Storeの掲載内容を同一リリースで扱い、**未公開機能を先に広告しない**という整合性条件を設定しました。実装担当のAIによる報告だけで公開判断せず、別AIのレビューおよび人間による受入・最終承認を組み合わせています。

## 実績の限界

小規模プロダクトの実践であり、エンタープライズレベルのSDLCや全端末・全アクセシビリティ項目の網羅的保証を構築したという主張ではありません。

**Requirements Governance・AI Orchestration・Traceability・Release Approval**
